---
title: Operação GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: A operação GetSharingFolder obtém o identificador de pasta local de uma pasta compartilhada especificada.
ms.openlocfilehash: 23adb10b22623fcbc1dd6b33bd674afafdaa8b19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823670"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="df7be-103">Operação GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="df7be-103">GetSharingFolder operation</span></span>

<span data-ttu-id="df7be-104">A operação **GetSharingFolder** obtém o identificador de pasta local de uma pasta compartilhada especificada.</span><span class="sxs-lookup"><span data-stu-id="df7be-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="df7be-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="df7be-105">SOAP Headers</span></span>

<span data-ttu-id="df7be-106">A operação **GetSharingFolder** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="df7be-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="df7be-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="df7be-107">**Header**</span></span>|<span data-ttu-id="df7be-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="df7be-108">**Element**</span></span>|<span data-ttu-id="df7be-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="df7be-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="df7be-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="df7be-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="df7be-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="df7be-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="df7be-112">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="df7be-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="df7be-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="df7be-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="df7be-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="df7be-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="df7be-115">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="df7be-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="df7be-116">Exemplo de solicitação de GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="df7be-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="df7be-117">Obtendo o identificador de pasta Local, especificando o elemento SharedFolderId da pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="df7be-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="df7be-118">O exemplo de código a seguir mostra como formar uma solicitação para obter o identificador da pasta local que corresponde à pasta que está sendo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="df7be-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="df7be-119">A pasta que está sendo compartilhada é identificada pelo endereço SMTP da caixa de correio que contém a pasta que está sendo compartilhada e pelo elemento [SharedFolderId](sharedfolderid.md) que representa o identificador nessa pasta.</span><span class="sxs-lookup"><span data-stu-id="df7be-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="df7be-120">Neste exemplo, a pasta que está sendo compartilhada pertence user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="df7be-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="df7be-121">Código</span><span class="sxs-lookup"><span data-stu-id="df7be-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="df7be-122">Obtendo o identificador de pasta Local, especificando o elemento de tipo de dados de pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="df7be-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="df7be-123">O exemplo de código a seguir mostra como formar uma solicitação para obter o identificador da pasta local que corresponde à pasta que está sendo compartilhada.</span><span class="sxs-lookup"><span data-stu-id="df7be-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="df7be-124">A pasta que está sendo compartilhada é identificada pelo endereço SMTP da caixa de correio que contém a pasta que está sendo compartilhada e por [DataType](datatype.md) elemento que representa o tipo de dados nessa pasta.</span><span class="sxs-lookup"><span data-stu-id="df7be-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="df7be-125">Neste exemplo, a pasta que está sendo compartilhada é a pasta de contatos que pertence ao user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="df7be-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="df7be-126">Código</span><span class="sxs-lookup"><span data-stu-id="df7be-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="df7be-127">Comments</span><span class="sxs-lookup"><span data-stu-id="df7be-127">Comments</span></span>

<span data-ttu-id="df7be-128">Para obter informações sobre os possíveis valores do elemento **DataType** , consulte [DataType](datatype.md).</span><span class="sxs-lookup"><span data-stu-id="df7be-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="df7be-129">GetSharingFolder de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="df7be-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="df7be-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7be-130">Description</span></span>

<span data-ttu-id="df7be-131">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="df7be-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="df7be-132">O atributo **Id** do elemento [SharingFolderId](sharingfolderid.md) representa o identificador da pasta local na relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="df7be-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="df7be-133">Código</span><span class="sxs-lookup"><span data-stu-id="df7be-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="df7be-134">Resposta de erro GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="df7be-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="df7be-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="df7be-135">Description</span></span>

<span data-ttu-id="df7be-136">O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="df7be-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="df7be-137">Neste exemplo, o erro ocorreu porque a solicitação especificado elementos [SharingFolderId](sharingfolderid.md) tanto o [tipo de dados](datatype.md) .</span><span class="sxs-lookup"><span data-stu-id="df7be-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="df7be-138">Observe que apenas um ou outro desses dois elementos pode ser especificado, mas não ambos.</span><span class="sxs-lookup"><span data-stu-id="df7be-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="df7be-139">Código</span><span class="sxs-lookup"><span data-stu-id="df7be-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="df7be-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="df7be-140">See also</span></span>



[<span data-ttu-id="df7be-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="df7be-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="df7be-142">GetSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="df7be-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="df7be-143">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="df7be-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="df7be-144">GetSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="df7be-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="df7be-145">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="df7be-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="df7be-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="df7be-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

