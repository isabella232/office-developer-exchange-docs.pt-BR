---
title: Propor um novo horário de reunião usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Descubra como proponham novos horários de seu aplicativo de cliente do Exchange usando o EWS no Exchange.
ms.openlocfilehash: f9edd8511332474a728635a6aa369a772da24786
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750807"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Propor um novo horário de reunião usando o EWS no Exchange

Descubra como proponham novos horários de seu aplicativo de cliente do Exchange usando o EWS no Exchange.
  
O novo recurso de tempo do propor habilita participantes proponham novos horários ao organizador da reunião como parte do fluxo de trabalho de calendário do Exchange. Quando um participante propõe uma nova reunião, o organizador pode usar o tempo de reunião novo proposto para atualizar a reunião e enviar atualizações a todos os participantes. Para poder habilitar propor novos horários de reunião de participantes, você precisa determinar se o organizador permite novas propostas de horários. Este artigo descreve como determinar se você pode propor um novo tempo e como usar o EWS para propor um novo horário.
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Determinar se você pode propor um novo horário para uma reunião usando o EWS
<a name="bk_Determine"> </a>

Antes de poder propor um novo horário para uma reunião, você precisará localizar uma referência a essa reunião e determinar se o organizador da reunião configurado para suportar novas propostas de horários na reunião. Você pode obter uma referência a uma reunião, seguindo um destes procedimentos: 
  
- Localizando a solicitação de reunião na caixa de entrada
    
- Localizando o compromisso do calendário
    
Use as etapas a seguir para localizar uma referência de reunião:
  
1. Use a operação de EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou o método de API gerenciada de EWS [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) ) para encontrar o alvo item de calendário ou de solicitação de reunião. Como alternativa, você pode usar a operação [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS para obter o identificador do destino de item de calendário ou de solicitação de reunião. 
    
2. Analise os resultados da operação **FindItem** (ou método **Folder.FindItems** ) para obter o identificador do item do item de reunião. 
    
3. Use a operação de EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) para obter os objetos de resposta para a reunião. 
    
O XML a seguir mostra o que é enviado para solicitar os objetos de resposta em um item.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

A resposta de operação **GetItem** terá uma aparência semelhante ao seguinte XML se você solicitar o identificador do item, o início da reunião e a hora de término, a coleção de objeto de resposta, e se o organizador permitir alterações proposto para o tempo de reunião. A coleção de objeto de resposta, que é representada por um elemento [ResponseObjects](http://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , contém o conjunto de respostas que são válidas para o item de calendário. O elemento **ProposeNewTime** é um objeto de resposta que indica que o usuário pode propor um novo horário para a reunião. Os elementos [AcceptItem](http://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx) [TentativelyAcceptItem](http://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)e [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) representam os objetos de resposta que você pode usar para propor um novo horário de reunião ao organizador da reunião. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Propor um novo horário de reunião usando o EWS
<a name="bk_Propose"> </a>

Se você tiver recebido um objeto de resposta **ProposeNewTime** quando você usou a operação **GetItem** para obter um item de calendário ou a solicitação de reunião, você pode responder com uma nova proposta hora de reunião. Se você não receber um objeto de resposta **ProposeNewTime** , você não conseguirá propor um novo horário de reunião como parte do fluxo de trabalho do calendário. No entanto, você poderá, respondê o organizador para solicitar um novo tempo de reunião. Se você receber um objeto de resposta **ProposeNewTime** , você pode responder à solicitação de reunião referenciando seu identificador e propor um novo horário de reunião do organizador. Isso é onde o objeto de resposta **ProposeNewTime** é diferente do que o padrão do objeto típico de resposta em que você não responder com um objeto de resposta **ProposeNewTime** . Você usar um dos outros objetos de resposta, como **AcceptItem**, **TentativelyAcceptItem**ou **DeclineItem**, proponham uma nova reunião da reunião. Este exemplo usa o objeto de resposta **AcceptItem** . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

A resposta à solicitação contém o identificador do item de calendário que foi adicionado ao calendário do participante e uma cópia da solicitação de reunião que foi colocada na pasta de itens excluídos do participante. A mensagem com a nova proposta de tempo de resposta também foi salvo na pasta de itens enviados do participante (você precisará encontrar a reunião mensagem de resposta para obter uma alça sobre ele).
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

O organizador receberá uma mensagem de [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) quando o participante responde com um novo tempo de reunião a proposta. A mensagem **MeetingResponse** contém a nova reunião proposta hora de início e hora de término e o identificador do item de calendário associado no calendário do organizador. O organizador pode usar essas informações para atualizar seus itens do calendário existentes para a reunião. Este é o fluxo de trabalho para o organizador responder a uma mensagem **MeetingResponse** que propõe um novo tempo de reunião: 
  
1. Determine se os elementos **ProposedStart** ou **ProposedEnd** foram definidos no **MeetingResponse**. Em caso afirmativo, vá para a etapa 2. Caso contrário, a mensagem **MeetingResponse** apenas indica se o nome do participante aceitou, aceitou provisoriamente ou recusou a reunião. 
    
2. Obtenha o item de calendário existente do organizador da reunião usando o identificador do EWS retornado no elemento **AssociatedCalendarItemId** . 
    
3. Compare os iniciar original e a hora de término com o tempo de reunião nova proposta. Se o tempo de reunião nova proposta é aceitável para o organizador, vá para a etapa 4. Caso contrário, o organizador da reunião pode ignorar o tempo de reunião proposto ou enviar uma resposta de email para o participante que proposto para o novo horário da reunião.
    
4. (Opcional) Realize uma chamada de operação do EWS [GetUserAvailability](http://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) para descobrir se o tempo proposto funcionará para todos os participantes, incluindo as caixas de correio de sala e recurso. (Você também pode usar o método de API gerenciada de EWS [ExchangeService.GetUserAvailability](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) para fazer isso.) 
    
5. Em seguida, o organizador pode atualizar sua reunião com os novos horários de reunião proposto e enviar as atualizações para todos os participantes, usando a operação de EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) (ou o método de API gerenciada de EWS [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) ). 
    
A figura a seguir mostra o processo que ocorre entre o organizador da reunião, o nome do participante e o servidor do Exchange que manipuladas as chamadas EWS.
  
**Figura 1. Processo para que propõe um novo tempo de reunião**

![A figura mostra o fluxo de trabalho entre o organizador, o Exchange e um participante quando um novo horário de reunião é proposto. Se o organizador permitir novas propostas de reuniões, um participante poderá propor um novo horário para a reunião com um objeto de resposta.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Diferenças de versão
<a name="bk_Behavior"> </a>

O novo recurso de tempo do propor foi introduzido na versão de compilação do Exchange 15.00.0800.007. Em versões anteriores do Exchange, os usuários de aplicativos do EWS tem que enviar um email separado para o organizador da reunião para solicitar um horário diferente. 
  
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Obtenha os compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

