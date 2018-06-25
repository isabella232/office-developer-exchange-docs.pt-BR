---
title: Verificando os resultados de uma chamada de EWS ou a API gerenciada de EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: Saiba como verificar os resultados de suas chamadas EWS ou a API gerenciada de EWS.
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750961"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>Verificando os resultados de uma chamada de EWS ou a API gerenciada de EWS

Saiba como verificar os resultados de suas chamadas EWS ou a API gerenciada de EWS.
  
Quando as coisas não estão funcionando corretamente, ele o ajuda a ver o que está acontecendo examinando as solicitações de SOAP que seu aplicativo está enviando através da rede e as respostas que o servidor está enviando novamente. O artigo de [Ferramentas e recursos para solucionar problemas de aplicativos do EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclui links para ferramentas para ajudar a capturar e exibir essas solicitações SOAP. Depois que você acaba de criar as solicitações e respostas, como verificar que a solicitação que é enviada ao servidor foi processada corretamente? Leia para descobrir. 
  
Se você estiver enviando solicitações EWS, você vai para iniciar sua verificação, verificando o atributo **ResponseClass** para cada mensagem de resposta na resposta. Que informará se a operação concluída com êxito em cada item. 
  
Dependendo do objeto seu método estiver chamando, se você estiver usando a API gerenciada de EWS para enviar solicitações, você pode fazer algumas verificação usando os objetos de resposta. Mas porque a resposta SOAP contém um subconjunto do que está incluído nos objetos de resposta da API gerenciada de EWS, talvez você queira examinar a resposta do SOAP. Como a resposta SOAP frequentemente pode conter mais informações do que os objetos de resposta do EWS Managed API, comece sua verificação com a resposta SOAP.
  
## <a name="verifying-the-results-of-a-soap-response"></a>Verificando os resultados de uma resposta SOAP
<a name="bk_verifysoap"> </a>

Quando você recebe uma resposta SOAP, a primeira coisa a ser analisado é o atributo **ResponseClass** . Este atributo é incluído em cada instância **ResponseMessageType** no elemento [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir. 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

Como uma resposta SOAP pode conter várias mensagens de resposta em uma única resposta SOAP, é importante verificar a cada mensagem de resposta individualmente.
  
Se você estiver trabalhando com uma operação que inclua um **ResponseClass** como parte da resposta da operação, como as seguintes, você poderá ficar tentado para verificar somente o **ResponseClass** da operação. 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

No entanto, o status de operação somente reflete a forma da resposta de nível superior e não reflete o status de todas as respostas de mensagem individual. No exemplo a seguir, a operação de [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**, mas o elemento [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) subjacente tem o valor de **erro** **ResponseClass** .
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Portanto para respostas EWS SOAP, você não pode depender do **ResponseClass** da operação – você tem a ser analisado o **ResponseClass** de cada mensagem de resposta para determinar se a operação encontrou quaisquer erros de processamento de itens. 
  
### <a name="verifying-success"></a>Verificando o sucesso

Se cada atributo **ResponseClass** para cada atributo **ResponseMessage** for definido com **sucesso**, a operação foi concluída com êxito em todos os itens, e você pode passar para a próxima tarefa.
  
O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) para recuperar um único item. Observe que, quando o **ResponseClass** estiver definida como **sucesso**, o associado [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) sempre é definida como **NoError**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

A seguir está uma resposta bem-sucedida a uma solicitação de operação **GetItem** para recuperar vários itens. Cada um dos elementos [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**.
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="handling-errors-and-warnings"></a>Tratando erros e avisos

Quando você recebe uma resposta e o atributo **ResponseClass** é definido para **Error**, a operação não foi concluída com êxito em um ou mais itens. Corrigir o problema e tentar novamente a sua solicitação ou a parte da sua solicitação que falhou. Um valor de atributo de valor de **Aviso** **ResponseClass** somente é retornado pela operação de [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) e indica que a entidade não pôde ser resolvida para uma identidade exclusiva. Você poderá ignorá-la para todas as outras operações. 
  
Em resposta a seguir, o atributo **ResponseClass** tem um valor de **erro**.
  
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

Neste exemplo, o EWS fornece dicas para depurar o problema. Quando o atributo **ResponseClass** tem um valor de **erro**, os seguintes elementos adicionais estão incluídos na resposta quando aplicável:
  
- [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — descreve o erro. 
    
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais. 
    
- [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifica os elementos que causou o erro. 
    
- [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — não utilizados. 
    
Você pode usar as informações fornecidas nesses elementos para investigar seu problema. No exemplo anterior, o **MessageText** indica que a propriedade não é válida para o tipo de objeto. A solicitação foi obter uma mensagem de email, mas o conjunto de propriedades incluído o **AssociatedCalendarItemId**, que só é válido para itens de compromisso.
  
O exemplo a seguir mostra um erro dizendo que foi recebido como parte de uma operação em lote para obter vários itens de email. O primeiro item foi recuperado com êxito e o **ResponseClass** é definido para o **sucesso**. O segundo item não pôde ser encontrado e o **ResponseClass** é definida para **Error**.
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Quando um ou mais itens em uma solicitação de lote não podem ser processadas, conforme solicitado, um erro será retornado para cada item que falharam e o restante dos itens no lote são processadas conforme o esperado. Falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado, ou se o item movido para uma pasta diferente e, portanto, tem uma nova ID de item. Porque a operação será Concluir para alguns itens e retornar um erro quando um ou mais itens não podem ser processadas, é importante verificar cada atributo **ResponseClass** antes de passar para a próxima operação. 
  
Se as informações fornecidas pelos elementos de resposta não ajudarem a corrigir sua solicitação ou caso contrário, desbloquear você, consulte as [próximas etapas](#bk_nextsteps).
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>Verificando os resultados de uma chamada de método de API gerenciada de EWS
<a name="bk_successful"> </a>

Se você estiver usando o EWS Managed API e chamar um método em um objeto de [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , seu método provavelmente retornará um objeto [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) , que contém uma coleção de objetos [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , ou uma coleção de objetos derivam de objetos **ServiceResponse** . Os objetos de **ServiceResponse** incluídos e o **ServiceResponseCollection** contêm informações sobre o resultado da chamada do método, você pode usar para verificar os resultados. 
  
Se você estiver usando o EWS Managed API e chamar um método em um objeto de [Item](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou um dos objetos derivados, o método provavelmente não retorna um objeto de resposta para verificar se há sucesso, mas lança uma [exceção](http://msdn.microsoft.com/EN-US/library/c18k6c59) se o método não for concluída. com êxito. 
  
### <a name="verifying-success"></a>Verificando o sucesso

Um dos benefícios do uso da API gerenciada de EWS é que ele fornece o status geral quando lidando com vários itens em uma resposta. Portanto, se o método que é chamado retornar um **ServiceResponseCollection**, você pode verificar se a propriedade [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) do **ServiceResponseCollection** for igual a [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Nesse caso, todos os itens no processo em lote foram concluídos com êxito; Você não precisa verificar cada objeto **ServiceResponse** individualmente. Se a propriedade **OverallResult** não está definida como **ServiceResult.Success**, você precisa [manipular o erro ou aviso](#bk_ewsmaerrors).
  
Se o método que você está chamando não retorna um **ServiceResponseCollection**, mas retornar um objeto de **ServiceResponse** , você precisa verificar o valor da propriedade **Result** . Se o valor de **resultado** é definido para o **sucesso**, você saberá o método concluído com êxito.
  
Se o método que você está chamando não tiver nenhum valor de retorno, não há realmente para verificar se há sucesso por meio da API gerenciada de EWS. Desde que uma exceção não é lançada, você pode assumir o método concluído com êxito. Para outras validações, você também pode [Verificar a resposta SOAP para verificar os resultados](#bk_verifysoap).
  
### <a name="handling-errors-warnings-and-exceptions"></a>Tratamento de erros, avisos e exceções
<a name="bk_ewsmaerrors"> </a>

Se seu código API gerenciada de EWS gera uma **exceção**, você pode usar o valor de [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) para determinar a origem do erro. A propriedade da **mensagem** contém o conteúdo do elemento [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) na resposta SOAP subjacente. Além disso, se a exceção é do tipo de objeto de [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , uma das exceções mais comuns, você também pode recuperar [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contidos no elemento SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) subjacente e a [resposta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) propriedade que identifica o objeto [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associado. O código a seguir mostra como capturar e exibir o conteúdo de um **ServiceResponseException**. 
  
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

Se o método que você chamou retornará um **ServiceResponseCollection**e o valor da propriedade **OverallResult** for igual a **Aviso** ou **erro**, você precisará percorrer o **ServiceResponseCollection** para cada objeto Encontre o erro. A propriedade **OverallResult** é definida como **Aviso** se pelo menos uma resposta tenha seu valor de **resultado** definido como **Aviso** e todas as outras respostas tem seus valores de **resultado** definidas para o **sucesso**. A propriedade **OverallResult** é definida como **erro** se pelo menos uma resposta tem seu valor de **resultado** definido como um **erro**. Quando o **OverallResult** estiver definido como **Aviso** ou **erro**, as seguintes propriedades são definidas nos objetos **ServiceResponse** conforme apropriado: 
  
- [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais. 
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — contém detalhes sobre o erro para alguns **ErrorCodes**. Por exemplo, quando o código de erro é **ErrorRecurrenceHasNoOccurrence**, o **ErrorDetails** irá conter chaves para **EffectiveStartDate** e **EffectiveEndDate**. 
    
- [ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — descreve o erro. 
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — se estiver disponível, identifica as propriedades que causou o erro. Por exemplo, quando o código de erro é **ErrorInvalidPropertyForOperation**, **ErrorProperties** contém a definição da propriedade que era inválida para a solicitação. 
    
- [Resultado](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contém **erro** ou **Aviso** quando algum problema for encontrado. 
    
Se as informações fornecidas pelas propriedades **ServiceResponse** não fornecem informações suficientes para corrigir a sua chamada de método ou desbloquear a você, consulte [próximas etapas](#bk_nextsteps) , procure por mais informações sobre valores de **ErrorCode** . 
  
## 
<a name="bk_nextsteps"> </a>

Você pode pesquisar informações de solução de problemas adicionais nos seguintes tópicos:
  
- Elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 
    
- Enumeração [ServiceError](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 
    
- [Erros relacionados a propriedade do EWS](ews-property-related-errors.md)
    
Além disso, dependendo da qual você está tentando realizar em sua solicitação, você pode encontrar informações úteis adicionais sobre o código de erro nos seguintes tópicos:
  
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)
    
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Tratando erros relacionados a exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

