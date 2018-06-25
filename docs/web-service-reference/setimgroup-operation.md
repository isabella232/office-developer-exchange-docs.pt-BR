---
title: Operação SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Encontre informações sobre o EWS SetImGroup operação.
ms.openlocfilehash: 80980c25888ab3fcae0a761e115c3ac3d578a013
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825421"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="f078b-103">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-103">SetImGroup operation</span></span>

<span data-ttu-id="f078b-104">Encontre informações sobre a operação de EWS **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f078b-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="f078b-105">A operação **SetImGroup** altera o nome de exibição de um grupo (IM) de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="f078b-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="f078b-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f078b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="f078b-107">Usando a operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="f078b-108">A operação **SetImGroup** só entra em um argumento de nome de exibição único.</span><span class="sxs-lookup"><span data-stu-id="f078b-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="f078b-109">Cabeçalhos SOAP SetImGroup operação</span><span class="sxs-lookup"><span data-stu-id="f078b-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="f078b-110">A operação **SetImGroup** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f078b-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="f078b-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="f078b-111">**Header name**</span></span>|<span data-ttu-id="f078b-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f078b-112">**Element**</span></span>|<span data-ttu-id="f078b-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f078b-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f078b-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="f078b-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="f078b-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f078b-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f078b-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="f078b-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="f078b-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f078b-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f078b-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="f078b-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="f078b-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f078b-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f078b-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f078b-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="f078b-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f078b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f078b-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="f078b-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f078b-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f078b-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f078b-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="f078b-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f078b-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f078b-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f078b-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="f078b-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f078b-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f078b-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f078b-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="f078b-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f078b-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f078b-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="f078b-130">Exemplo de solicitação de operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-130">SetImGroup operation request example</span></span>

<span data-ttu-id="f078b-131">O exemplo a seguir de uma solicitação de operação **SetImGroup** mostra como alterar um nome de exibição do grupo de mensagens Instantâneas para "MyNewGroupName".</span><span class="sxs-lookup"><span data-stu-id="f078b-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f078b-132">O identificador de repositório do Exchange foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f078b-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f078b-133">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="f078b-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f078b-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="f078b-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="f078b-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="f078b-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="f078b-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="f078b-137">Resposta de operação SetImGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f078b-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="f078b-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f078b-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="f078b-139">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="f078b-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f078b-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f078b-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="f078b-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f078b-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="f078b-142">Resposta de erro de operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-142">SetImGroup operation error response</span></span>

<span data-ttu-id="f078b-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f078b-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="f078b-144">A seguinte resposta de erro ocorre quando é feita uma tentativa para alterar o nome de exibição do grupo para o nome de exibição do grupo existente.</span><span class="sxs-lookup"><span data-stu-id="f078b-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="f078b-145">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="f078b-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f078b-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f078b-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="f078b-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="f078b-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f078b-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f078b-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f078b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f078b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="f078b-150">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="f078b-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f078b-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="f078b-151">See also</span></span>

- [<span data-ttu-id="f078b-152">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f078b-152">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="f078b-153">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="f078b-154">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="f078b-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

