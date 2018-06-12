---
title: Operação RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Encontre informações sobre o EWS RemoveImGroup operação.
ms.openlocfilehash: 85b312f0b156125a2d5395658ccea06d831abdde
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825097"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="0e479-103">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-103">RemoveImGroup operation</span></span>

<span data-ttu-id="0e479-104">Encontre informações sobre a operação de EWS **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="0e479-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="0e479-105">A operação **RemoveImGroup** remove um único grupo de (IM) mensagens instantâneo uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0e479-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="0e479-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0e479-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="0e479-107">Usando a operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="0e479-108">A operação **RemoveImGroup** só entra em um argumento de identificador único grupo.</span><span class="sxs-lookup"><span data-stu-id="0e479-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="0e479-109">Cabeçalhos SOAP RemoveImGroup operação</span><span class="sxs-lookup"><span data-stu-id="0e479-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="0e479-110">A operação **RemoveImGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0e479-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0e479-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="0e479-111">**Header name**</span></span>|<span data-ttu-id="0e479-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e479-112">**Element**</span></span>|<span data-ttu-id="0e479-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e479-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0e479-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="0e479-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0e479-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0e479-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0e479-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="0e479-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0e479-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e479-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0e479-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0e479-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0e479-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0e479-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0e479-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0e479-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0e479-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e479-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0e479-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0e479-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0e479-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0e479-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0e479-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="0e479-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0e479-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e479-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0e479-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0e479-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0e479-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0e479-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0e479-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e479-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0e479-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0e479-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="0e479-130">Exemplo de solicitação de operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="0e479-131">O exemplo a seguir de uma solicitação de operação **RemoveImGroup** mostra como remover um grupo de mensagens Instantâneas.</span><span class="sxs-lookup"><span data-stu-id="0e479-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0e479-132">A ID de grupo foi reduzida para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0e479-132">The group ID has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="0e479-133">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0e479-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0e479-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="0e479-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="0e479-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="0e479-136">Resposta de operação RemoveImGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0e479-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="0e479-137">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="0e479-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0e479-138">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0e479-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0e479-139">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0e479-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="0e479-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0e479-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="0e479-141">Operação RemoveImGroup ErrorInvalidImGroupId resposta de erro</span><span class="sxs-lookup"><span data-stu-id="0e479-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="0e479-142">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="0e479-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="0e479-143">A seguinte resposta de erro ocorre quando é feita uma tentativa para remover um grupo que não existe na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0e479-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0e479-144">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0e479-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0e479-145">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0e479-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="0e479-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="0e479-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0e479-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0e479-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0e479-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0e479-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="0e479-149">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="0e479-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="0e479-150">Operação RemoveImGroup ErrorInvalidIdMalformed resposta de erro</span><span class="sxs-lookup"><span data-stu-id="0e479-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="0e479-151">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="0e479-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="0e479-152">A seguinte resposta de erro ocorre quando é feita uma tentativa para remover um grupo com um identificador de grupo formatado incorretamente.</span><span class="sxs-lookup"><span data-stu-id="0e479-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0e479-153">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0e479-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0e479-154">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0e479-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="0e479-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="0e479-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0e479-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0e479-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0e479-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0e479-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0e479-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e479-158">See also</span></span>

- [<span data-ttu-id="0e479-159">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0e479-159">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="0e479-160">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="0e479-161">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="0e479-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

