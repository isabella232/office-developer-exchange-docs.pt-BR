---
title: Verificar os resultados de uma chamada de API gerenciada do EWS ou EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Saiba como verificar os resultados das chamadas da API gerenciada do EWS ou do EWS.
localization_priority: Priority
ms.openlocfilehash: be8e76898dd111a6dec33d4a57d9d50a2a935390
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457393"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Verificar os resultados de uma chamada de API gerenciada do EWS ou EWS

Saiba como verificar os resultados das chamadas da API gerenciada do EWS ou do EWS.
  
Quando as coisas não estão funcionando corretamente, ele ajuda a ver o que está acontecendo examinando as solicitações SOAP que seu aplicativo está enviando pela rede e as respostas que o servidor está enviando de volta. O artigo [ferramentas e recursos para solução de problemas de aplicativos do EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclui links para ferramentas para ajudar a capturar e exibir essas solicitações SOAP. Depois de ter recebido as solicitações e as respostas, como verificar se a solicitação enviada ao servidor foi processada corretamente? Leia para saber mais. 
  
Se você estiver enviando solicitações do EWS, será iniciada a verificação verificando o atributo **ResponseClass** para cada mensagem de resposta na resposta. Isso indicará se a operação foi concluída com êxito em cada item. 
  
Dependendo do objeto que seu método está chamando, se você estiver usando a API gerenciada do EWS para enviar solicitações, poderá fazer alguma verificação usando os objetos Response. Mas como a resposta SOAP contém um superconjunto do que está incluído nos objetos de resposta da API gerenciada do EWS, convém também examinar a resposta SOAP. Como a resposta SOAP geralmente pode conter mais informações do que os objetos de resposta da API gerenciada do EWS, inicie a verificação com a resposta SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Verificar os resultados de uma resposta SOAP
<a name="bk_verifysoap"> </a>

Ao receber uma resposta SOAP, a primeira coisa a ser examinada é o atributo **ResponseClass** . Esse atributo é incluído em cada instância do **ResponseMessageType** no elemento [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Como uma resposta SOAP pode conter várias mensagens de resposta em uma única resposta SOAP, é importante verificar cada mensagem de resposta individualmente.
  
Se você estiver trabalhando com uma operação que inclui um **ResponseClass** como parte da resposta de operação, como o seguinte, talvez você tenha tentado apenas verificar o **ResponseClass** da operação. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

No entanto, o status da operação só reflete a forma da resposta de nível superior e não reflete o status de todas as respostas de mensagem individuais. No exemplo a seguir, a operação [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) tem um **ResponseClass** de **êxito**, mas o elemento [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) subjacente tem um valor de **ResponseClass** de **erro**.
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

Portanto, para as respostas do EWS do SOAP, não é possível confiar no **ResponseClass** da operação: você precisa examinar o **ResponseClass** de cada mensagem de resposta para determinar se a operação encontrou erros de processamento dos itens. 
  
### <a name="verifying-success"></a>Verificando o sucesso

Se cada atributo **ResponseClass** para cada atributo **ResponseMessage** for definido como **êxito**, a operação será concluída com êxito em todos os itens e você poderá passar para a próxima tarefa.
  
O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) para recuperar um único item. Observe que, quando **ResponseClass** é definido como **Success**, o [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) associado é sempre definido como **NOERROR**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

A seguir está uma resposta bem-sucedida para uma solicitação de operação **GetItem** para recuperar vários itens. Cada um dos elementos [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a>Tratamento de erros e avisos

Quando você recebe uma resposta e o atributo **ResponseClass** está definido como **erro**, a operação não foi concluída com êxito em um ou mais itens. Corrija o problema e repita a solicitação ou a parte da solicitação que falhou. Um valor de atributo **ResponseClass** do valor de **aviso** só é retornado pela operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) e indica que a entidade não pôde ser resolvida para uma identidade exclusiva. Você pode ignorá-lo para todas as outras operações. 
  
Na resposta a seguir, o atributo **ResponseClass** tem um valor de **erro**.
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

Neste exemplo, o EWS fornece pistas para depurar o problema. Quando o atributo **ResponseClass** tem um valor de **erro**, os seguintes elementos adicionais são incluídos na resposta quando aplicável:
  
- [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — descreve o erro. 
    
- [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais. 
    
- [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifica os elementos que causaram o erro. 
    
- [DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — não usado. 
    
Você pode usar as informações fornecidas nesses elementos para investigar seu problema. No exemplo anterior, o **MessageText** indica que a propriedade não é válida para o tipo de objeto. A solicitação era obter uma mensagem de email, mas o conjunto de propriedades incluía o **AssociatedCalendarItemId**, que é válido apenas para itens de compromisso.
  
O exemplo a seguir mostra um erro que foi recebido como parte de uma operação em lote para obter vários itens de email. O primeiro item foi recuperado com êxito e o **ResponseClass** está definido como **Success**. O segundo item não pôde ser encontrado e o **ResponseClass** está definido como **erro**.
  
```XML
<m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

Quando um ou mais itens em uma solicitação em lote não puderem ser processados como solicitados, um erro será retornado para cada item que falhou e o restante dos itens no lote será processado conforme o esperado. As falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado ou quando o item é movido para uma pasta diferente e, portanto, tem uma nova ID de item. Como a operação será concluída para alguns itens e não retornar um erro quando um ou mais itens não puderem ser processados, é importante verificar cada atributo **ResponseClass** antes de passar para a próxima operação. 
  
Se as informações fornecidas pelos elementos Response não ajudarem você a corrigir sua solicitação ou desbloqueá-lo, consulte [as próximas etapas](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Verificando os resultados de uma chamada de método de API gerenciada do EWS
<a name="bk_successful"> </a>

Se você estiver usando a API gerenciada do EWS e chamando um método em um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , o método provavelmente retornará um objeto [perresponsecollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) , que contém uma coleção de objetos de [imresposta](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , ou uma coleção de objetos derivados dos objetos de **WebResponse** . Os **objetos de** **imresponsecollection** e inclusos contêm informações sobre o resultado da chamada do método, que você pode usar para verificar os resultados. 
  
Se você estiver usando a API gerenciada do EWS e chamando um método em um objeto [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou um dos objetos derivados, o método provavelmente não retornará um objeto Response para verificar o sucesso, mas gerará uma [exceção](https://msdn.microsoft.com/library/c18k6c59) se o método não for concluído com êxito. 
  
### <a name="verifying-success"></a>Verificando o sucesso

Uma vantagem de usar a API gerenciada do EWS é que ela fornece um status geral ao lidar com vários itens em uma resposta. Portanto, se o método que você chamou retornar um **Perresponsecollection**, você pode verificar se a propriedade [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de **myresponsecollection** é igual a [falha. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Em caso afirmativo, todos os itens no processo em lote foram concluídos com êxito; Você não precisa verificar cada objeto de **WebResponse** individualmente. Se a propriedade **OverallResult** não estiver definida como **imresult. Success**, você terá que [lidar com o erro ou aviso](#bk_ewsmaerrors).
  
Se o método que você está chamando não retornar um **Perresponsecollection**, mas retornar um objeto de **inresponse** , você precisará verificar o valor da propriedade **Result** . Se o valor do **resultado** for definido como **êxito**, você saberá que o método foi concluído com êxito.
  
Se o método que você está chamando não tem valor de retorno, não há uma maneira de verificar o sucesso por meio da API gerenciada do EWS. Contanto que uma exceção não seja lançada, você pode supor que o método foi concluído com êxito. Para validação adicional, você também pode [verificar a resposta SOAP para verificar os resultados](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Tratamento de erros, avisos e exceções
<a name="bk_ewsmaerrors"> </a>

Se o código de API gerenciada do EWS gerar uma **exceção**, você poderá usar o valor [Exception. Message](https://msdn.microsoft.com/library/9btwf6wk) para determinar a origem do erro. A propriedade **Message** contém o conteúdo do elemento [MESSAGETEXT](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) na resposta SOAP subjacente. Além disso, se a exceção for do tipo de objeto de [Inresponseexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , uma das exceções mais comuns, você também poderá recuperar o [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contido no elemento SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) subjacente e a propriedade [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) que identifica o objeto de [inresponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associado. O código a seguir mostra como capturar e exibir o conteúdo **de um.** 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

Se o método que você chamou retornar um **Perresponsecollection**e o valor da propriedade **OverallResult** for igual a **aviso** ou **erro**, você terá que executar um loop em cada objeto no **perresponsecollection** para localizar o erro. A propriedade **OverallResult** é definida como **aviso** se pelo menos uma resposta tiver seu valor de **resultado** definido como **aviso** e todas as outras respostas tiverem seus valores de **resultado** definidos como **êxito**. A propriedade **OverallResult** é definida como **erro** se pelo menos uma resposta tiver seu valor de **resultado** definido como **erro**. Quando o **OverallResult** é definido como **aviso** ou **erro**, as seguintes propriedades são definidas nos objetos de **inresponse** , conforme apropriado: 
  
- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais. 
    
- [ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — contém detalhes sobre o erro para alguns **errorCodes**. Por exemplo, quando o código de erro for **ErrorRecurrenceHasNoOccurrence**, o **ErrorDetails** conterá chaves para **EffectiveStartDate** e **EffectiveEndDate**. 
    
- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — descreve o erro. 
    
- [Errorproperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — se disponível, identifica as propriedades que causaram o erro. Por exemplo, quando o código de erro é **ErrorInvalidPropertyForOperation**, **errorproperties** contém a definição da propriedade que era inválida para a solicitação. 
    
- [Resultado](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contém **erro** ou **aviso** quando um problema é encontrado. 
    
Se as informações fornecidas pelas propriedades de **myresponse** não fornecerem informações suficientes para corrigir a chamada de método ou desbloquear você, consulte [as próximas etapas](#bk_nextsteps) para se aprofundar em valores de **ErrorCode** . 
  
## 
<a name="bk_nextsteps"> </a>

Você pode pesquisar informações adicionais de solução de problemas nos seguintes tópicos:
  
- Elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- Enumeração de [erro](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
    
- [Erros relacionados à propriedade do EWS](ews-property-related-errors.md)
    
Além disso, dependendo do que você está tentando realizar em sua solicitação, você pode encontrar informações úteis adicionais sobre o código de erro nos seguintes tópicos:
  
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
- [Tratamento de erros relacionados à notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Como lidar com erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratamento de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

