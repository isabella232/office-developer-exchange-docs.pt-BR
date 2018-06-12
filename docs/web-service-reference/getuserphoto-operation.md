---
title: Operação GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Encontre informações sobre o EWS GetUserPhoto operação.
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823694"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="1cde1-103">Operação GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="1cde1-103">GetUserPhoto operation</span></span>

<span data-ttu-id="1cde1-104">Encontre informações sobre a operação de EWS **GetUserPhoto** .</span><span class="sxs-lookup"><span data-stu-id="1cde1-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="1cde1-105">A operação **GetUserPhoto** obtém uma foto do usuário dos serviços de domínio Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="1cde1-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="1cde1-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1cde1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="1cde1-107">Usando a operação GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="1cde1-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="1cde1-108">A operação de **RemoveContactFromImList** é uma operação simple que aceita o endereço de email do usuário e o tamanho da foto solicitado e retorna o fluxo de foto na resposta.</span><span class="sxs-lookup"><span data-stu-id="1cde1-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1cde1-109">EWS tem um SOAP e uma operação baseado em REST para obter as fotos dos usuários.</span><span class="sxs-lookup"><span data-stu-id="1cde1-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="1cde1-110">Para obter informações sobre a interface REST, consulte [obter fotos de usuário usando o EWS no Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1cde1-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="1cde1-111">Cabeçalhos SOAP GetUserPhoto operação</span><span class="sxs-lookup"><span data-stu-id="1cde1-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="1cde1-112">A operação **GetUserPhoto** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1cde1-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1cde1-113">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="1cde1-113">**Header name**</span></span>|<span data-ttu-id="1cde1-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1cde1-114">**Element**</span></span>|<span data-ttu-id="1cde1-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1cde1-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1cde1-116">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1cde1-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1cde1-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1cde1-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1cde1-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="1cde1-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1cde1-119">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cde1-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1cde1-120">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1cde1-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1cde1-121">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1cde1-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1cde1-122">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cde1-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1cde1-123">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1cde1-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="1cde1-124">Exemplo de solicitação de operação GetUserPhoto: Obtenha a foto do usuário</span><span class="sxs-lookup"><span data-stu-id="1cde1-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="1cde1-125">O exemplo a seguir de uma solicitação de operação **GetUserPhoto** mostra como obter a foto do usuário.</span><span class="sxs-lookup"><span data-stu-id="1cde1-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="1cde1-126">Este exemplo solicita uma foto do usuário 48x48 pixels.</span><span class="sxs-lookup"><span data-stu-id="1cde1-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1cde1-127">Os seguintes elementos são usados na solicitação de corpo SOAP:</span><span class="sxs-lookup"><span data-stu-id="1cde1-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="1cde1-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="1cde1-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="1cde1-129">Email (String)</span><span class="sxs-lookup"><span data-stu-id="1cde1-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="1cde1-130">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="1cde1-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="1cde1-131">Resposta de operação GetUserPhoto bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="1cde1-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="1cde1-132">O exemplo a seguir mostra uma resposta bem-sucedida a uma operação **GetUserPhoto** para obter a foto do usuário.</span><span class="sxs-lookup"><span data-stu-id="1cde1-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="1cde1-133">Os seguintes elementos são usados no corpo SOAP de resposta:</span><span class="sxs-lookup"><span data-stu-id="1cde1-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="1cde1-134">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="1cde1-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="1cde1-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1cde1-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1cde1-136">HasChanged</span><span class="sxs-lookup"><span data-stu-id="1cde1-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="1cde1-137">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="1cde1-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="1cde1-138">Resposta de erro de operação GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="1cde1-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="1cde1-139">O envelope SOAP não retornará um código de erro, se for feita uma tentativa para obter uma foto do usuário para um endereço de email que não existe na organização.</span><span class="sxs-lookup"><span data-stu-id="1cde1-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="1cde1-140">Um código de status HTTP 500 será retornado na resposta para indicar que a solicitação foi bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="1cde1-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1cde1-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="1cde1-141">See also</span></span>

- [<span data-ttu-id="1cde1-142">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1cde1-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="1cde1-143">Obtenha as fotos de usuários usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1cde1-143">Get user photos by using EWS in Exchange</span></span>](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

