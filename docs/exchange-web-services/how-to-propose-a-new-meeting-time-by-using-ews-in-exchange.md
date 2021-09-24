---
title: Propor um novo horário de reunião usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Saiba como propor novos horários de reunião do seu aplicativo cliente Exchange usando o EWS em Exchange.
ms.openlocfilehash: a6406aaef2005e74165e647510af891d2a59503e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522226"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Propor um novo horário de reunião usando o EWS no Exchange

Saiba como propor novos horários de reunião do seu aplicativo cliente Exchange usando o EWS em Exchange.
  
O recurso propor novo horário permite que os participantes proporem novos horários de reunião ao organizador da reunião como parte do fluxo de trabalho Exchange calendário. Quando um participante propõe uma nova reunião, o organizador pode usar o novo horário de reunião proposto para atualizar a reunião e enviar atualizações para todos os participantes. Antes de permitir que os participantes proporem novos horários de reunião, você precisa determinar se o organizador permite novas propostas de horário. Este artigo descreve como determinar se você pode propor um novo horário e como usar o EWS para propor um novo horário.
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Determinar se você pode propor um novo horário para uma reunião usando o EWS
<a name="bk_Determine"> </a>

Antes de propor um novo horário para uma reunião, você precisa encontrar uma referência para essa reunião e determinar se o organizador da reunião configurou a reunião para dar suporte a novas propostas de tempo. Você pode obter uma referência a uma reunião fazendo um dos seguintes: 
  
- Localizar a solicitação de reunião na Caixa de Entrada
    
- Localizar o compromisso no calendário
    
Use as etapas a seguir para encontrar uma referência de reunião:
  
1. Use a [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (ou o [método Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API) para encontrar a solicitação de reunião de destino ou o item de calendário. Como alternativa, você pode usar a operação [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS para obter o identificador da solicitação de reunião de destino ou do item de calendário. 
    
2. Analisar os resultados da operação **FindItem** (ou **método Folder.FindItems)** para obter o identificador de item do item de reunião. 
    
3. Use a [operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS para obter os objetos de resposta da reunião. 
    
O XML a seguir mostra o que é enviado para solicitar os objetos de resposta em um item.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

A resposta da operação **GetItem** será semelhante ao XML a seguir se você solicitar o identificador de item, o início e a hora de término da reunião, a coleção de objetos de resposta e se o organizador permitir alterações propostas para o horário da reunião. A coleção de objetos de resposta, que é representada pelo [elemento ResponseObjects,](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) contém o conjunto de respostas que são válidas para o item de calendário. O **elemento ProposeNewTime** é um objeto de resposta que indica que o usuário pode propor um novo horário para a reunião. Os [elementos AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)e [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) representam os objetos de resposta que você pode usar para propor um novo horário de reunião ao organizador da reunião. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Se você recebeu um objeto de resposta **ProposeNewTime** quando usou a operação **GetItem** para obter um item de calendário ou uma solicitação de reunião, você poderá responder com um novo horário de reunião proposto. Se você não recebeu um objeto de resposta **ProposeNewTime,** não poderá propor um novo horário de reunião como parte do fluxo de trabalho do calendário. No entanto, você pode responder ao organizador para solicitar um novo horário de reunião. Se você receber um objeto de resposta **ProposeNewTime,** poderá responder à reunião fazendo referência ao identificador e propor um novo horário de reunião ao organizador. É aqui que o objeto de resposta **ProposeNewTime** é diferente do padrão de objeto de resposta típico em que você não responde com um objeto de resposta **ProposeNewTime.** Você usa um dos outros objetos de resposta de reunião, como **AcceptItem**, **TentativelyAcceptItem** ou **DeclineItem,** para propor uma nova reunião. Este exemplo usa o **objeto de resposta AcceptItem.** 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

A resposta a essa solicitação contém o identificador do item de calendário que foi adicionado ao calendário do participante e uma cópia da solicitação de reunião que foi colocada na pasta Itens Excluídos do participante. A mensagem de resposta com a proposta de nova hora também foi salva na pasta Itens Enviados do participante (você precisará encontrar a mensagem de resposta da reunião para obter uma alça sobre ela).
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

O organizador receberá uma [mensagem MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) quando o participante responder com um novo horário de reunião proposto. A **mensagem MeetingResponse** contém a nova hora e a hora de término da reunião propostas e o identificador do item de calendário associado no calendário do organizador. O organizador pode usar essas informações para atualizar seu item de calendário existente para a reunião. Veja a seguir o fluxo de trabalho para o organizador responder a uma mensagem **MeetingResponse** que propõe um novo horário de reunião: 
  
1. Determinar se os **elementos ProposedStart** **ou ProposedEnd** foram definidos no **MeetingResponse**. Em caso afirmado, vá para a etapa 2. Caso não seja, a mensagem **MeetingResponse** indica apenas se o participante aceitou, aceitou ou recusou a reunião. 
    
2. Obter o item de calendário existente do organizador para a reunião usando o identificador EWS retornado no **elemento AssociatedCalendarItemId.** 
    
3. Compare o início e a hora de término originais com o novo horário de reunião proposto. Se o novo horário de reunião proposto for aceitável para o organizador, vá para a etapa 4. Caso contrário, o organizador da reunião pode ignorar o horário de reunião proposto ou enviar uma resposta de email para o participante que propunha o novo horário da reunião.
    
4. (Opcional) Execute uma [chamada de operação GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS para descobrir se o horário proposto funcionará para todos os participantes, incluindo caixas de correio de sala e recursos. (Você também pode usar o método api gerenciada do [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS para fazer isso.) 
    
5. Em seguida, o organizador pode atualizar sua reunião com os novos horários de reunião propostos e enviar as atualizações para todos os participantes usando a operação [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (ou o [método Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) EWS Managed API). 
    
A figura a seguir mostra o processo que ocorre entre o organizador da reunião, o participante e o servidor Exchange que manipulava as chamadas EWS.
  
**Figura 1. Processo para propor um novo horário de reunião**

![A figura mostra o fluxo de trabalho entre o organizador, o Exchange e um participante quando um novo horário de reunião é proposto. Se o organizador permitir novas propostas de reuniões, um participante poderá propor um novo horário para a reunião com um objeto de resposta.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Diferenças de versão
<a name="bk_Behavior"> </a>

O recurso propor novo horário foi introduzido Exchange versão de com build 15.00.0800.007. Em versões anteriores do Exchange, os usuários do aplicativo EWS têm que enviar um email separado ao organizador da reunião para solicitar um horário de reunião diferente. 
  
## <a name="see-also"></a>Confira também


- [Calendários e EWS no Exchange](calendars-and-ews-in-exchange.md)
    
- [Criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

