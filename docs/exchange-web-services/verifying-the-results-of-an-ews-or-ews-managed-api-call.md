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
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="8f380-103">Verificando os resultados de uma chamada de EWS ou a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="8f380-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="8f380-104">Saiba como verificar os resultados de suas chamadas EWS ou a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="8f380-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="8f380-105">Quando as coisas não estão funcionando corretamente, ele o ajuda a ver o que está acontecendo examinando as solicitações de SOAP que seu aplicativo está enviando através da rede e as respostas que o servidor está enviando novamente.</span><span class="sxs-lookup"><span data-stu-id="8f380-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="8f380-106">O artigo de [Ferramentas e recursos para solucionar problemas de aplicativos do EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclui links para ferramentas para ajudar a capturar e exibir essas solicitações SOAP.</span><span class="sxs-lookup"><span data-stu-id="8f380-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="8f380-107">Depois que você acaba de criar as solicitações e respostas, como verificar que a solicitação que é enviada ao servidor foi processada corretamente?</span><span class="sxs-lookup"><span data-stu-id="8f380-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="8f380-108">Leia para descobrir.</span><span class="sxs-lookup"><span data-stu-id="8f380-108">Read on to find out.</span></span> 
  
<span data-ttu-id="8f380-109">Se você estiver enviando solicitações EWS, você vai para iniciar sua verificação, verificando o atributo **ResponseClass** para cada mensagem de resposta na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f380-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="8f380-110">Que informará se a operação concluída com êxito em cada item.</span><span class="sxs-lookup"><span data-stu-id="8f380-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="8f380-111">Dependendo do objeto seu método estiver chamando, se você estiver usando a API gerenciada de EWS para enviar solicitações, você pode fazer algumas verificação usando os objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f380-111">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects.</span></span> <span data-ttu-id="8f380-112">Mas porque a resposta SOAP contém um subconjunto do que está incluído nos objetos de resposta da API gerenciada de EWS, talvez você queira examinar a resposta do SOAP.</span><span class="sxs-lookup"><span data-stu-id="8f380-112">But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well.</span></span> <span data-ttu-id="8f380-113">Como a resposta SOAP frequentemente pode conter mais informações do que os objetos de resposta do EWS Managed API, comece sua verificação com a resposta SOAP.</span><span class="sxs-lookup"><span data-stu-id="8f380-113">Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="8f380-114">Verificando os resultados de uma resposta SOAP</span><span class="sxs-lookup"><span data-stu-id="8f380-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="8f380-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="8f380-115"></span></span>

<span data-ttu-id="8f380-116">Quando você recebe uma resposta SOAP, a primeira coisa a ser analisado é o atributo **ResponseClass** .</span><span class="sxs-lookup"><span data-stu-id="8f380-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="8f380-117">Este atributo é incluído em cada instância **ResponseMessageType** no elemento [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8f380-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="8f380-118">Como uma resposta SOAP pode conter várias mensagens de resposta em uma única resposta SOAP, é importante verificar a cada mensagem de resposta individualmente.</span><span class="sxs-lookup"><span data-stu-id="8f380-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="8f380-119">Se você estiver trabalhando com uma operação que inclua um **ResponseClass** como parte da resposta da operação, como as seguintes, você poderá ficar tentado para verificar somente o **ResponseClass** da operação.</span><span class="sxs-lookup"><span data-stu-id="8f380-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="8f380-120">No entanto, o status de operação somente reflete a forma da resposta de nível superior e não reflete o status de todas as respostas de mensagem individual.</span><span class="sxs-lookup"><span data-stu-id="8f380-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="8f380-121">No exemplo a seguir, a operação de [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**, mas o elemento [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) subjacente tem o valor de **erro** **ResponseClass** .</span><span class="sxs-lookup"><span data-stu-id="8f380-121">In the following example, the [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
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

<span data-ttu-id="8f380-122">Portanto para respostas EWS SOAP, você não pode depender do **ResponseClass** da operação – você tem a ser analisado o **ResponseClass** de cada mensagem de resposta para determinar se a operação encontrou quaisquer erros de processamento de itens.</span><span class="sxs-lookup"><span data-stu-id="8f380-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="8f380-123">Verificando o sucesso</span><span class="sxs-lookup"><span data-stu-id="8f380-123">Verifying success</span></span>

<span data-ttu-id="8f380-124">Se cada atributo **ResponseClass** para cada atributo **ResponseMessage** for definido com **sucesso**, a operação foi concluída com êxito em todos os itens, e você pode passar para a próxima tarefa.</span><span class="sxs-lookup"><span data-stu-id="8f380-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="8f380-125">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) para recuperar um único item.</span><span class="sxs-lookup"><span data-stu-id="8f380-125">The following example shows a successful response to a [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="8f380-126">Observe que, quando o **ResponseClass** estiver definida como **sucesso**, o associado [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) sempre é definida como **NoError**.</span><span class="sxs-lookup"><span data-stu-id="8f380-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
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

<span data-ttu-id="8f380-127">A seguir está uma resposta bem-sucedida a uma solicitação de operação **GetItem** para recuperar vários itens.</span><span class="sxs-lookup"><span data-stu-id="8f380-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="8f380-128">Cada um dos elementos [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**.</span><span class="sxs-lookup"><span data-stu-id="8f380-128">Each of the [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
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

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="8f380-129">Tratando erros e avisos</span><span class="sxs-lookup"><span data-stu-id="8f380-129">Handling errors and warnings</span></span>

<span data-ttu-id="8f380-130">Quando você recebe uma resposta e o atributo **ResponseClass** é definido para **Error**, a operação não foi concluída com êxito em um ou mais itens.</span><span class="sxs-lookup"><span data-stu-id="8f380-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="8f380-131">Corrigir o problema e tentar novamente a sua solicitação ou a parte da sua solicitação que falhou.</span><span class="sxs-lookup"><span data-stu-id="8f380-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="8f380-132">Um valor de atributo de valor de **Aviso** **ResponseClass** somente é retornado pela operação de [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) e indica que a entidade não pôde ser resolvida para uma identidade exclusiva.</span><span class="sxs-lookup"><span data-stu-id="8f380-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="8f380-133">Você poderá ignorá-la para todas as outras operações.</span><span class="sxs-lookup"><span data-stu-id="8f380-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="8f380-134">Em resposta a seguir, o atributo **ResponseClass** tem um valor de **erro**.</span><span class="sxs-lookup"><span data-stu-id="8f380-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
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

<span data-ttu-id="8f380-135">Neste exemplo, o EWS fornece dicas para depurar o problema.</span><span class="sxs-lookup"><span data-stu-id="8f380-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="8f380-136">Quando o atributo **ResponseClass** tem um valor de **erro**, os seguintes elementos adicionais estão incluídos na resposta quando aplicável:</span><span class="sxs-lookup"><span data-stu-id="8f380-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="8f380-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="8f380-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="8f380-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="8f380-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifica os elementos que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="8f380-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — não utilizados.</span><span class="sxs-lookup"><span data-stu-id="8f380-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="8f380-141">Você pode usar as informações fornecidas nesses elementos para investigar seu problema.</span><span class="sxs-lookup"><span data-stu-id="8f380-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="8f380-142">No exemplo anterior, o **MessageText** indica que a propriedade não é válida para o tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="8f380-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="8f380-143">A solicitação foi obter uma mensagem de email, mas o conjunto de propriedades incluído o **AssociatedCalendarItemId**, que só é válido para itens de compromisso.</span><span class="sxs-lookup"><span data-stu-id="8f380-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="8f380-144">O exemplo a seguir mostra um erro dizendo que foi recebido como parte de uma operação em lote para obter vários itens de email.</span><span class="sxs-lookup"><span data-stu-id="8f380-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="8f380-145">O primeiro item foi recuperado com êxito e o **ResponseClass** é definido para o **sucesso**.</span><span class="sxs-lookup"><span data-stu-id="8f380-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="8f380-146">O segundo item não pôde ser encontrado e o **ResponseClass** é definida para **Error**.</span><span class="sxs-lookup"><span data-stu-id="8f380-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
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

<span data-ttu-id="8f380-147">Quando um ou mais itens em uma solicitação de lote não podem ser processadas, conforme solicitado, um erro será retornado para cada item que falharam e o restante dos itens no lote são processadas conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="8f380-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="8f380-148">Falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado, ou se o item movido para uma pasta diferente e, portanto, tem uma nova ID de item.</span><span class="sxs-lookup"><span data-stu-id="8f380-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="8f380-149">Porque a operação será Concluir para alguns itens e retornar um erro quando um ou mais itens não podem ser processadas, é importante verificar cada atributo **ResponseClass** antes de passar para a próxima operação.</span><span class="sxs-lookup"><span data-stu-id="8f380-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="8f380-150">Se as informações fornecidas pelos elementos de resposta não ajudarem a corrigir sua solicitação ou caso contrário, desbloquear você, consulte as [próximas etapas](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="8f380-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="8f380-151">Verificando os resultados de uma chamada de método de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="8f380-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="8f380-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="8f380-152"></span></span>

<span data-ttu-id="8f380-153">Se você estiver usando o EWS Managed API e chamar um método em um objeto de [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , seu método provavelmente retornará um objeto [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) , que contém uma coleção de objetos [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , ou uma coleção de objetos derivam de objetos **ServiceResponse** .</span><span class="sxs-lookup"><span data-stu-id="8f380-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="8f380-154">Os objetos de **ServiceResponse** incluídos e o **ServiceResponseCollection** contêm informações sobre o resultado da chamada do método, você pode usar para verificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="8f380-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="8f380-155">Se você estiver usando o EWS Managed API e chamar um método em um objeto de [Item](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou um dos objetos derivados, o método provavelmente não retorna um objeto de resposta para verificar se há sucesso, mas lança uma [exceção](http://msdn.microsoft.com/EN-US/library/c18k6c59) se o método não for concluída. com êxito.</span><span class="sxs-lookup"><span data-stu-id="8f380-155">If you're using the EWS Managed API and calling a method on an [Item](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](http://msdn.microsoft.com/EN-US/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="8f380-156">Verificando o sucesso</span><span class="sxs-lookup"><span data-stu-id="8f380-156">Verifying success</span></span>

<span data-ttu-id="8f380-157">Um dos benefícios do uso da API gerenciada de EWS é que ele fornece o status geral quando lidando com vários itens em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8f380-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="8f380-158">Portanto, se o método que é chamado retornar um **ServiceResponseCollection**, você pode verificar se a propriedade [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) do **ServiceResponseCollection** for igual a [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8f380-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="8f380-159">Nesse caso, todos os itens no processo em lote foram concluídos com êxito; Você não precisa verificar cada objeto **ServiceResponse** individualmente.</span><span class="sxs-lookup"><span data-stu-id="8f380-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="8f380-160">Se a propriedade **OverallResult** não está definida como **ServiceResult.Success**, você precisa [manipular o erro ou aviso](#bk_ewsmaerrors).</span><span class="sxs-lookup"><span data-stu-id="8f380-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="8f380-161">Se o método que você está chamando não retorna um **ServiceResponseCollection**, mas retornar um objeto de **ServiceResponse** , você precisa verificar o valor da propriedade **Result** .</span><span class="sxs-lookup"><span data-stu-id="8f380-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="8f380-162">Se o valor de **resultado** é definido para o **sucesso**, você saberá o método concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="8f380-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="8f380-163">Se o método que você está chamando não tiver nenhum valor de retorno, não há realmente para verificar se há sucesso por meio da API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="8f380-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="8f380-164">Desde que uma exceção não é lançada, você pode assumir o método concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="8f380-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="8f380-165">Para outras validações, você também pode [Verificar a resposta SOAP para verificar os resultados](#bk_verifysoap).</span><span class="sxs-lookup"><span data-stu-id="8f380-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="8f380-166">Tratamento de erros, avisos e exceções</span><span class="sxs-lookup"><span data-stu-id="8f380-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="8f380-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="8f380-167"></span></span>

<span data-ttu-id="8f380-168">Se seu código API gerenciada de EWS gera uma **exceção**, você pode usar o valor de [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) para determinar a origem do erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="8f380-169">A propriedade da **mensagem** contém o conteúdo do elemento [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) na resposta SOAP subjacente.</span><span class="sxs-lookup"><span data-stu-id="8f380-169">The **Message** property contains the contents of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="8f380-170">Além disso, se a exceção é do tipo de objeto de [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , uma das exceções mais comuns, você também pode recuperar [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contidos no elemento SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) subjacente e a [resposta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) propriedade que identifica o objeto [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associado.</span><span class="sxs-lookup"><span data-stu-id="8f380-170">In addition, if the exception is of type [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="8f380-171">O código a seguir mostra como capturar e exibir o conteúdo de um **ServiceResponseException**.</span><span class="sxs-lookup"><span data-stu-id="8f380-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
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

<span data-ttu-id="8f380-172">Se o método que você chamou retornará um **ServiceResponseCollection**e o valor da propriedade **OverallResult** for igual a **Aviso** ou **erro**, você precisará percorrer o **ServiceResponseCollection** para cada objeto Encontre o erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="8f380-173">A propriedade **OverallResult** é definida como **Aviso** se pelo menos uma resposta tenha seu valor de **resultado** definido como **Aviso** e todas as outras respostas tem seus valores de **resultado** definidas para o **sucesso**.</span><span class="sxs-lookup"><span data-stu-id="8f380-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="8f380-174">A propriedade **OverallResult** é definida como **erro** se pelo menos uma resposta tem seu valor de **resultado** definido como um **erro**.</span><span class="sxs-lookup"><span data-stu-id="8f380-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="8f380-175">Quando o **OverallResult** estiver definido como **Aviso** ou **erro**, as seguintes propriedades são definidas nos objetos **ServiceResponse** conforme apropriado:</span><span class="sxs-lookup"><span data-stu-id="8f380-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="8f380-176">[ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="8f380-176">[ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="8f380-177">[ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — contém detalhes sobre o erro para alguns **ErrorCodes**.</span><span class="sxs-lookup"><span data-stu-id="8f380-177">[ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="8f380-178">Por exemplo, quando o código de erro é **ErrorRecurrenceHasNoOccurrence**, o **ErrorDetails** irá conter chaves para **EffectiveStartDate** e **EffectiveEndDate**.</span><span class="sxs-lookup"><span data-stu-id="8f380-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="8f380-179">[ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-179">[ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="8f380-180">[ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — se estiver disponível, identifica as propriedades que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="8f380-180">[ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="8f380-181">Por exemplo, quando o código de erro é **ErrorInvalidPropertyForOperation**, **ErrorProperties** contém a definição da propriedade que era inválida para a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f380-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="8f380-182">[Resultado](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contém **erro** ou **Aviso** quando algum problema for encontrado.</span><span class="sxs-lookup"><span data-stu-id="8f380-182">[Result](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="8f380-183">Se as informações fornecidas pelas propriedades **ServiceResponse** não fornecem informações suficientes para corrigir a sua chamada de método ou desbloquear a você, consulte [próximas etapas](#bk_nextsteps) , procure por mais informações sobre valores de **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="8f380-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="8f380-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="8f380-184"></span></span>

<span data-ttu-id="8f380-185">Você pode pesquisar informações de solução de problemas adicionais nos seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="8f380-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="8f380-186">Elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="8f380-186">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="8f380-187">Enumeração [ServiceError](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="8f380-187">[ServiceError](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="8f380-188">Erros relacionados a propriedade do EWS</span><span class="sxs-lookup"><span data-stu-id="8f380-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="8f380-189">Além disso, dependendo da qual você está tentando realizar em sua solicitação, você pode encontrar informações úteis adicionais sobre o código de erro nos seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="8f380-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="8f380-190">Manipulação de mensagens de erro de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="8f380-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="8f380-191">Tratando erros relacionados a notificação no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f380-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8f380-192">Tratando erros relacionados a sincronização no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f380-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8f380-193">Tratando erros relacionados a exclusão no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f380-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="8f380-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f380-194">See also</span></span>


- [<span data-ttu-id="8f380-195">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="8f380-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="8f380-196">Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="8f380-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

