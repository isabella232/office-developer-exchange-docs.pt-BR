---
title: Operação RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Encontre informações sobre a operação do EWS do RemoveImGroup.
ms.openlocfilehash: b5e38404cbb1907a1118ab3ae8e56abb5a8d5e41
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456720"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="c4ca9-103">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-103">RemoveImGroup operation</span></span>

<span data-ttu-id="c4ca9-104">Encontre informações sobre a operação do EWS do **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="c4ca9-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="c4ca9-105">A operação **RemoveImGroup** remove um único grupo de mensagens instantâneas (IM) de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="c4ca9-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="c4ca9-107">Usando a operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="c4ca9-108">A operação **RemoveImGroup** aceita apenas um único argumento identificador de grupo.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="c4ca9-109">Cabeçalhos SOAP de operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="c4ca9-110">A operação **RemoveImGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c4ca9-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-111">**Header name**</span></span>|<span data-ttu-id="c4ca9-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-112">**Element**</span></span>|<span data-ttu-id="c4ca9-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c4ca9-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c4ca9-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c4ca9-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c4ca9-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="c4ca9-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c4ca9-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c4ca9-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c4ca9-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c4ca9-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="c4ca9-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c4ca9-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c4ca9-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c4ca9-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c4ca9-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c4ca9-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c4ca9-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c4ca9-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c4ca9-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c4ca9-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c4ca9-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c4ca9-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="c4ca9-130">Exemplo de solicitação de operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="c4ca9-131">O exemplo a seguir de uma solicitação de operação **RemoveImGroup** mostra como remover um grupo de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c4ca9-132">A ID do grupo foi reduzida para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-132">The group ID has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c4ca9-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c4ca9-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c4ca9-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="c4ca9-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="c4ca9-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="c4ca9-136">Resposta de operação RemoveImGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c4ca9-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="c4ca9-137">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="c4ca9-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c4ca9-138">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c4ca9-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c4ca9-139">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="c4ca9-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="c4ca9-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c4ca9-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="c4ca9-141">Resposta de erro ErrorInvalidImGroupId operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="c4ca9-142">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="c4ca9-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="c4ca9-143">A seguinte resposta de erro ocorre quando é feita uma tentativa de remover um grupo que não existe na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c4ca9-144">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c4ca9-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c4ca9-145">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="c4ca9-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="c4ca9-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="c4ca9-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c4ca9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c4ca9-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c4ca9-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c4ca9-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="c4ca9-149">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="c4ca9-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="c4ca9-150">Resposta de erro ErrorInvalidIdMalformed operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="c4ca9-151">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="c4ca9-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="c4ca9-152">A seguinte resposta de erro ocorre quando é feita uma tentativa de remover um grupo com um identificador de grupo formatado incorretamente.</span><span class="sxs-lookup"><span data-stu-id="c4ca9-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c4ca9-153">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="c4ca9-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c4ca9-154">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="c4ca9-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="c4ca9-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="c4ca9-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c4ca9-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c4ca9-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c4ca9-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c4ca9-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="c4ca9-158">Também consulte</span><span class="sxs-lookup"><span data-stu-id="c4ca9-158">See also</span></span>

- [<span data-ttu-id="c4ca9-159">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c4ca9-159">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="c4ca9-160">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="c4ca9-161">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="c4ca9-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

