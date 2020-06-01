---
title: Operação SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Encontre informações sobre a operação do EWS do SetImGroup.
ms.openlocfilehash: 37b290559fff0b2de57669741547ba4b1b56c28c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438072"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="e2633-103">Operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-103">SetImGroup operation</span></span>

<span data-ttu-id="e2633-104">Encontre informações sobre a operação do EWS do **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="e2633-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="e2633-105">A operação **SetImGroup** altera o nome de exibição de um grupo de mensagens instantâneas (IM).</span><span class="sxs-lookup"><span data-stu-id="e2633-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="e2633-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e2633-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="e2633-107">Usando a operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="e2633-108">A operação **SetImGroup** usa apenas um único argumento de nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e2633-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="e2633-109">Cabeçalhos SOAP de operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="e2633-110">A operação **SetImGroup** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e2633-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e2633-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="e2633-111">**Header name**</span></span>|<span data-ttu-id="e2633-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2633-112">**Element**</span></span>|<span data-ttu-id="e2633-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2633-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e2633-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="e2633-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="e2633-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e2633-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e2633-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="e2633-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="e2633-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2633-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e2633-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="e2633-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="e2633-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="e2633-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e2633-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e2633-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="e2633-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2633-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e2633-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e2633-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e2633-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e2633-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e2633-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="e2633-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e2633-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2633-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e2633-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e2633-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e2633-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e2633-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e2633-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2633-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e2633-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e2633-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="e2633-130">Exemplo de solicitação de operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-130">SetImGroup operation request example</span></span>

<span data-ttu-id="e2633-131">O exemplo a seguir de uma solicitação de operação **SetImGroup** mostra como alterar o nome de exibição de um grupo de mensagens instantâneas para "MyNewGroupName".</span><span class="sxs-lookup"><span data-stu-id="e2633-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e2633-132">O identificador do repositório do Exchange foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2633-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e2633-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="e2633-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e2633-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="e2633-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="e2633-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="e2633-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2633-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="e2633-137">Resposta de operação SetImGroup bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="e2633-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="e2633-138">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="e2633-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="e2633-139">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="e2633-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e2633-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="e2633-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="e2633-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e2633-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="e2633-142">Resposta de erro de operação SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-142">SetImGroup operation error response</span></span>

<span data-ttu-id="e2633-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="e2633-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="e2633-144">A seguinte resposta de erro ocorre quando é feita uma tentativa de alterar o nome de exibição do grupo para o nome de exibição do grupo existente.</span><span class="sxs-lookup"><span data-stu-id="e2633-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e2633-145">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="e2633-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e2633-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="e2633-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="e2633-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="e2633-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e2633-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e2633-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e2633-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e2633-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="e2633-150">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="e2633-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e2633-151">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e2633-151">See also</span></span>

- [<span data-ttu-id="e2633-152">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2633-152">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="e2633-153">Operação AddImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="e2633-154">Operação RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="e2633-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

