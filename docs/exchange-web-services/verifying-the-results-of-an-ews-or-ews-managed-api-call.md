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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457393"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="c8b02-103">Verificar os resultados de uma chamada de API gerenciada do EWS ou EWS</span><span class="sxs-lookup"><span data-stu-id="c8b02-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="c8b02-104">Saiba como verificar os resultados das chamadas da API gerenciada do EWS ou do EWS.</span><span class="sxs-lookup"><span data-stu-id="c8b02-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="c8b02-105">Quando as coisas não estão funcionando corretamente, ele ajuda a ver o que está acontecendo examinando as solicitações SOAP que seu aplicativo está enviando pela rede e as respostas que o servidor está enviando de volta.</span><span class="sxs-lookup"><span data-stu-id="c8b02-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="c8b02-106">O artigo [ferramentas e recursos para solução de problemas de aplicativos do EWS](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) inclui links para ferramentas para ajudar a capturar e exibir essas solicitações SOAP.</span><span class="sxs-lookup"><span data-stu-id="c8b02-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="c8b02-107">Depois de ter recebido as solicitações e as respostas, como verificar se a solicitação enviada ao servidor foi processada corretamente?</span><span class="sxs-lookup"><span data-stu-id="c8b02-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="c8b02-108">Leia para saber mais.</span><span class="sxs-lookup"><span data-stu-id="c8b02-108">Read on to find out.</span></span> 
  
<span data-ttu-id="c8b02-109">Se você estiver enviando solicitações do EWS, será iniciada a verificação verificando o atributo **ResponseClass** para cada mensagem de resposta na resposta.</span><span class="sxs-lookup"><span data-stu-id="c8b02-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="c8b02-110">Isso indicará se a operação foi concluída com êxito em cada item.</span><span class="sxs-lookup"><span data-stu-id="c8b02-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="c8b02-111">Dependendo do objeto que seu método está chamando, se você estiver usando a API gerenciada do EWS para enviar solicitações, poderá fazer alguma verificação usando os objetos Response.</span><span class="sxs-lookup"><span data-stu-id="c8b02-111">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects.</span></span> <span data-ttu-id="c8b02-112">Mas como a resposta SOAP contém um superconjunto do que está incluído nos objetos de resposta da API gerenciada do EWS, convém também examinar a resposta SOAP.</span><span class="sxs-lookup"><span data-stu-id="c8b02-112">But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well.</span></span> <span data-ttu-id="c8b02-113">Como a resposta SOAP geralmente pode conter mais informações do que os objetos de resposta da API gerenciada do EWS, inicie a verificação com a resposta SOAP.</span><span class="sxs-lookup"><span data-stu-id="c8b02-113">Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="c8b02-114">Verificar os resultados de uma resposta SOAP</span><span class="sxs-lookup"><span data-stu-id="c8b02-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="c8b02-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="c8b02-115"><a name="bk_verifysoap"> </a></span></span>

<span data-ttu-id="c8b02-116">Ao receber uma resposta SOAP, a primeira coisa a ser examinada é o atributo **ResponseClass** .</span><span class="sxs-lookup"><span data-stu-id="c8b02-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="c8b02-117">Esse atributo é incluído em cada instância do **ResponseMessageType** no elemento [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="c8b02-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="c8b02-118">Como uma resposta SOAP pode conter várias mensagens de resposta em uma única resposta SOAP, é importante verificar cada mensagem de resposta individualmente.</span><span class="sxs-lookup"><span data-stu-id="c8b02-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="c8b02-119">Se você estiver trabalhando com uma operação que inclui um **ResponseClass** como parte da resposta de operação, como o seguinte, talvez você tenha tentado apenas verificar o **ResponseClass** da operação.</span><span class="sxs-lookup"><span data-stu-id="c8b02-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="c8b02-120">No entanto, o status da operação só reflete a forma da resposta de nível superior e não reflete o status de todas as respostas de mensagem individuais.</span><span class="sxs-lookup"><span data-stu-id="c8b02-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="c8b02-121">No exemplo a seguir, a operação [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) tem um **ResponseClass** de **êxito**, mas o elemento [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) subjacente tem um valor de **ResponseClass** de **erro**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-121">In the following example, the [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
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

<span data-ttu-id="c8b02-122">Portanto, para as respostas do EWS do SOAP, não é possível confiar no **ResponseClass** da operação: você precisa examinar o **ResponseClass** de cada mensagem de resposta para determinar se a operação encontrou erros de processamento dos itens.</span><span class="sxs-lookup"><span data-stu-id="c8b02-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="c8b02-123">Verificando o sucesso</span><span class="sxs-lookup"><span data-stu-id="c8b02-123">Verifying success</span></span>

<span data-ttu-id="c8b02-124">Se cada atributo **ResponseClass** para cada atributo **ResponseMessage** for definido como **êxito**, a operação será concluída com êxito em todos os itens e você poderá passar para a próxima tarefa.</span><span class="sxs-lookup"><span data-stu-id="c8b02-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="c8b02-125">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) para recuperar um único item.</span><span class="sxs-lookup"><span data-stu-id="c8b02-125">The following example shows a successful response to a [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="c8b02-126">Observe que, quando **ResponseClass** é definido como **Success**, o [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) associado é sempre definido como **NOERROR**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
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

<span data-ttu-id="c8b02-127">A seguir está uma resposta bem-sucedida para uma solicitação de operação **GetItem** para recuperar vários itens.</span><span class="sxs-lookup"><span data-stu-id="c8b02-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="c8b02-128">Cada um dos elementos [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) tem um **ResponseClass** de **sucesso**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-128">Each of the [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
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

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="c8b02-129">Tratamento de erros e avisos</span><span class="sxs-lookup"><span data-stu-id="c8b02-129">Handling errors and warnings</span></span>

<span data-ttu-id="c8b02-130">Quando você recebe uma resposta e o atributo **ResponseClass** está definido como **erro**, a operação não foi concluída com êxito em um ou mais itens.</span><span class="sxs-lookup"><span data-stu-id="c8b02-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="c8b02-131">Corrija o problema e repita a solicitação ou a parte da solicitação que falhou.</span><span class="sxs-lookup"><span data-stu-id="c8b02-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="c8b02-132">Um valor de atributo **ResponseClass** do valor de **aviso** só é retornado pela operação [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) e indica que a entidade não pôde ser resolvida para uma identidade exclusiva.</span><span class="sxs-lookup"><span data-stu-id="c8b02-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="c8b02-133">Você pode ignorá-lo para todas as outras operações.</span><span class="sxs-lookup"><span data-stu-id="c8b02-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="c8b02-134">Na resposta a seguir, o atributo **ResponseClass** tem um valor de **erro**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
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

<span data-ttu-id="c8b02-135">Neste exemplo, o EWS fornece pistas para depurar o problema.</span><span class="sxs-lookup"><span data-stu-id="c8b02-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="c8b02-136">Quando o atributo **ResponseClass** tem um valor de **erro**, os seguintes elementos adicionais são incluídos na resposta quando aplicável:</span><span class="sxs-lookup"><span data-stu-id="c8b02-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="c8b02-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="c8b02-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="c8b02-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="c8b02-139">[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — identifica os elementos que causaram o erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-139">[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="c8b02-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — não usado.</span><span class="sxs-lookup"><span data-stu-id="c8b02-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="c8b02-141">Você pode usar as informações fornecidas nesses elementos para investigar seu problema.</span><span class="sxs-lookup"><span data-stu-id="c8b02-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="c8b02-142">No exemplo anterior, o **MessageText** indica que a propriedade não é válida para o tipo de objeto.</span><span class="sxs-lookup"><span data-stu-id="c8b02-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="c8b02-143">A solicitação era obter uma mensagem de email, mas o conjunto de propriedades incluía o **AssociatedCalendarItemId**, que é válido apenas para itens de compromisso.</span><span class="sxs-lookup"><span data-stu-id="c8b02-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="c8b02-144">O exemplo a seguir mostra um erro que foi recebido como parte de uma operação em lote para obter vários itens de email.</span><span class="sxs-lookup"><span data-stu-id="c8b02-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="c8b02-145">O primeiro item foi recuperado com êxito e o **ResponseClass** está definido como **Success**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="c8b02-146">O segundo item não pôde ser encontrado e o **ResponseClass** está definido como **erro**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
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

<span data-ttu-id="c8b02-147">Quando um ou mais itens em uma solicitação em lote não puderem ser processados como solicitados, um erro será retornado para cada item que falhou e o restante dos itens no lote será processado conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="c8b02-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="c8b02-148">As falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado ou quando o item é movido para uma pasta diferente e, portanto, tem uma nova ID de item.</span><span class="sxs-lookup"><span data-stu-id="c8b02-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="c8b02-149">Como a operação será concluída para alguns itens e não retornar um erro quando um ou mais itens não puderem ser processados, é importante verificar cada atributo **ResponseClass** antes de passar para a próxima operação.</span><span class="sxs-lookup"><span data-stu-id="c8b02-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="c8b02-150">Se as informações fornecidas pelos elementos Response não ajudarem você a corrigir sua solicitação ou desbloqueá-lo, consulte [as próximas etapas](#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="c8b02-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="c8b02-151">Verificando os resultados de uma chamada de método de API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="c8b02-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="c8b02-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="c8b02-152"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="c8b02-153">Se você estiver usando a API gerenciada do EWS e chamando um método em um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , o método provavelmente retornará um objeto [perresponsecollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) , que contém uma coleção de objetos de [imresposta](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) , ou uma coleção de objetos derivados dos objetos de **WebResponse** .</span><span class="sxs-lookup"><span data-stu-id="c8b02-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="c8b02-154">Os **objetos de** **imresponsecollection** e inclusos contêm informações sobre o resultado da chamada do método, que você pode usar para verificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="c8b02-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="c8b02-155">Se você estiver usando a API gerenciada do EWS e chamando um método em um objeto [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , ou um dos objetos derivados, o método provavelmente não retornará um objeto Response para verificar o sucesso, mas gerará uma [exceção](https://msdn.microsoft.com/library/c18k6c59) se o método não for concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="c8b02-155">If you're using the EWS Managed API and calling a method on an [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](https://msdn.microsoft.com/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="c8b02-156">Verificando o sucesso</span><span class="sxs-lookup"><span data-stu-id="c8b02-156">Verifying success</span></span>

<span data-ttu-id="c8b02-157">Uma vantagem de usar a API gerenciada do EWS é que ela fornece um status geral ao lidar com vários itens em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c8b02-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="c8b02-158">Portanto, se o método que você chamou retornar um **Perresponsecollection**, você pode verificar se a propriedade [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de **myresponsecollection** é igual a [falha. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c8b02-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="c8b02-159">Em caso afirmativo, todos os itens no processo em lote foram concluídos com êxito; Você não precisa verificar cada objeto de **WebResponse** individualmente.</span><span class="sxs-lookup"><span data-stu-id="c8b02-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="c8b02-160">Se a propriedade **OverallResult** não estiver definida como **imresult. Success**, você terá que [lidar com o erro ou aviso](#bk_ewsmaerrors).</span><span class="sxs-lookup"><span data-stu-id="c8b02-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="c8b02-161">Se o método que você está chamando não retornar um **Perresponsecollection**, mas retornar um objeto de **inresponse** , você precisará verificar o valor da propriedade **Result** .</span><span class="sxs-lookup"><span data-stu-id="c8b02-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="c8b02-162">Se o valor do **resultado** for definido como **êxito**, você saberá que o método foi concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="c8b02-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="c8b02-163">Se o método que você está chamando não tem valor de retorno, não há uma maneira de verificar o sucesso por meio da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="c8b02-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="c8b02-164">Contanto que uma exceção não seja lançada, você pode supor que o método foi concluído com êxito.</span><span class="sxs-lookup"><span data-stu-id="c8b02-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="c8b02-165">Para validação adicional, você também pode [verificar a resposta SOAP para verificar os resultados](#bk_verifysoap).</span><span class="sxs-lookup"><span data-stu-id="c8b02-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="c8b02-166">Tratamento de erros, avisos e exceções</span><span class="sxs-lookup"><span data-stu-id="c8b02-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="c8b02-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="c8b02-167"><a name="bk_ewsmaerrors"> </a></span></span>

<span data-ttu-id="c8b02-168">Se o código de API gerenciada do EWS gerar uma **exceção**, você poderá usar o valor [Exception. Message](https://msdn.microsoft.com/library/9btwf6wk) para determinar a origem do erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](https://msdn.microsoft.com/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="c8b02-169">A propriedade **Message** contém o conteúdo do elemento [MESSAGETEXT](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) na resposta SOAP subjacente.</span><span class="sxs-lookup"><span data-stu-id="c8b02-169">The **Message** property contains the contents of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="c8b02-170">Além disso, se a exceção for do tipo de objeto de [Inresponseexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) , uma das exceções mais comuns, você também poderá recuperar o [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contido no elemento SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) subjacente e a propriedade [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) que identifica o objeto de [inresponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) associado.</span><span class="sxs-lookup"><span data-stu-id="c8b02-170">In addition, if the exception is of type [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="c8b02-171">O código a seguir mostra como capturar e exibir o conteúdo **de um.**</span><span class="sxs-lookup"><span data-stu-id="c8b02-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
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

<span data-ttu-id="c8b02-172">Se o método que você chamou retornar um **Perresponsecollection**e o valor da propriedade **OverallResult** for igual a **aviso** ou **erro**, você terá que executar um loop em cada objeto no **perresponsecollection** para localizar o erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="c8b02-173">A propriedade **OverallResult** é definida como **aviso** se pelo menos uma resposta tiver seu valor de **resultado** definido como **aviso** e todas as outras respostas tiverem seus valores de **resultado** definidos como **êxito**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="c8b02-174">A propriedade **OverallResult** é definida como **erro** se pelo menos uma resposta tiver seu valor de **resultado** definido como **erro**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="c8b02-175">Quando o **OverallResult** é definido como **aviso** ou **erro**, as seguintes propriedades são definidas nos objetos de **inresponse** , conforme apropriado:</span><span class="sxs-lookup"><span data-stu-id="c8b02-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="c8b02-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — contém o código de erro, que pode ser usado para localizar recursos de solução de problemas adicionais.</span><span class="sxs-lookup"><span data-stu-id="c8b02-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="c8b02-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — contém detalhes sobre o erro para alguns **errorCodes**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="c8b02-178">Por exemplo, quando o código de erro for **ErrorRecurrenceHasNoOccurrence**, o **ErrorDetails** conterá chaves para **EffectiveStartDate** e **EffectiveEndDate**.</span><span class="sxs-lookup"><span data-stu-id="c8b02-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="c8b02-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — descreve o erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="c8b02-180">[Errorproperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — se disponível, identifica as propriedades que causaram o erro.</span><span class="sxs-lookup"><span data-stu-id="c8b02-180">[ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="c8b02-181">Por exemplo, quando o código de erro é **ErrorInvalidPropertyForOperation**, **errorproperties** contém a definição da propriedade que era inválida para a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8b02-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="c8b02-182">[Resultado](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — contém **erro** ou **aviso** quando um problema é encontrado.</span><span class="sxs-lookup"><span data-stu-id="c8b02-182">[Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="c8b02-183">Se as informações fornecidas pelas propriedades de **myresponse** não fornecerem informações suficientes para corrigir a chamada de método ou desbloquear você, consulte [as próximas etapas](#bk_nextsteps) para se aprofundar em valores de **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="c8b02-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="c8b02-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="c8b02-184"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="c8b02-185">Você pode pesquisar informações adicionais de solução de problemas nos seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="c8b02-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="c8b02-186">Elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c8b02-186">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="c8b02-187">Enumeração de [erro](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="c8b02-187">[ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="c8b02-188">Erros relacionados à propriedade do EWS</span><span class="sxs-lookup"><span data-stu-id="c8b02-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="c8b02-189">Além disso, dependendo do que você está tentando realizar em sua solicitação, você pode encontrar informações úteis adicionais sobre o código de erro nos seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="c8b02-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="c8b02-190">Manipulação de mensagens de erro de Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="c8b02-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="c8b02-191">Tratamento de erros relacionados à notificação no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8b02-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="c8b02-192">Como lidar com erros relacionados à sincronização no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8b02-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="c8b02-193">Tratamento de erros relacionados à exclusão no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8b02-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="c8b02-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8b02-194">See also</span></span>


- [<span data-ttu-id="c8b02-195">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="c8b02-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="c8b02-196">Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="c8b02-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

