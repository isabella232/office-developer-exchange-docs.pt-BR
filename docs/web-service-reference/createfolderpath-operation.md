---
title: Operação CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: Encontre informações sobre o EWS CreateFolderPath operação.
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751587"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="bb9bf-103">Operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="bb9bf-103">CreateFolderPath operation</span></span>

<span data-ttu-id="bb9bf-104">Encontre informações sobre a operação de EWS **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="bb9bf-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="bb9bf-105">A operação **CreateFolderPath** cria uma hierarquia de pastas.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="bb9bf-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="bb9bf-107">Usando a operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="bb9bf-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="bb9bf-108">A solicitação de operação **CreateFolderPath** adota uma matriz de pastas e um identificador de pasta pai e cria uma hierarquia de pastas com base na ordem as pastas na matriz.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="bb9bf-109">Cabeçalhos SOAP CreateFolderPath operação</span><span class="sxs-lookup"><span data-stu-id="bb9bf-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="bb9bf-110">A operação **CreateFolderPath** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bb9bf-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-111">**Header name**</span></span>|<span data-ttu-id="bb9bf-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-112">**Element**</span></span>|<span data-ttu-id="bb9bf-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bb9bf-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="bb9bf-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="bb9bf-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="bb9bf-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="bb9bf-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bb9bf-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="bb9bf-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="bb9bf-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="bb9bf-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="bb9bf-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bb9bf-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bb9bf-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="bb9bf-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bb9bf-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bb9bf-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bb9bf-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bb9bf-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bb9bf-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bb9bf-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bb9bf-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="bb9bf-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="bb9bf-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="bb9bf-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="bb9bf-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="bb9bf-132">Identifica o escopo de fuso horário para as propriedades de **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="bb9bf-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="bb9bf-133">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="bb9bf-134">Exemplo de solicitação de operação CreateFolderPath: criar uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="bb9bf-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="bb9bf-135">O exemplo a seguir de uma solicitação de operação **CreateFolderPath** mostra como criar uma hierarquia de pastas é três pastas profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bb9bf-136">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:CreateFolderPath>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ParentFolderId>
         <m:RelativeFolderPath>
            <t:Folder>
               <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MySecondLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
            </t:Folder>
         </m:RelativeFolderPath>
      </m:CreateFolderPath>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bb9bf-137">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bb9bf-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb9bf-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="bb9bf-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="bb9bf-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="bb9bf-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="bb9bf-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="bb9bf-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="bb9bf-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="bb9bf-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="bb9bf-142">Folder</span><span class="sxs-lookup"><span data-stu-id="bb9bf-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="bb9bf-143">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="bb9bf-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="bb9bf-144">Resposta de operação CreateFolderPath bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="bb9bf-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="bb9bf-145">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **CreateFolderPath** para criar uma pasta pastas de hierarquia três profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExYisXAAA=" ChangeKey="AQAAABYAABq6Wxb"/>
                     <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExm4QrAABqxisYAAA=" ChangeKey="AQAAABYAAAm4QrAABq6Wxg"/>
                     <t:DisplayName>MySecondLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTAABqxisZAAA=" ChangeKey="AQAAABYAA6Wxl"/>
                     <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bb9bf-146">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bb9bf-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb9bf-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="bb9bf-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="bb9bf-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bb9bf-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bb9bf-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bb9bf-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="bb9bf-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bb9bf-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bb9bf-151">Pastas</span><span class="sxs-lookup"><span data-stu-id="bb9bf-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="bb9bf-152">Folder</span><span class="sxs-lookup"><span data-stu-id="bb9bf-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="bb9bf-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="bb9bf-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="bb9bf-154">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="bb9bf-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="bb9bf-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bb9bf-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="bb9bf-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="bb9bf-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="bb9bf-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="bb9bf-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="bb9bf-158">Resposta de erro de operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="bb9bf-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="bb9bf-159">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="bb9bf-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="bb9bf-160">Esta é uma resposta a uma solicitação para criar duas pastas, a primeira delas não possuem uma propriedade de nome de exibição definido.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="bb9bf-161">A primeira pasta na hierarquia não pode ser criada sem uma propriedade de nome de exibição e a segunda pasta não pode ser criada porque a pasta pai na hierarquia não foi criada.</span><span class="sxs-lookup"><span data-stu-id="bb9bf-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The folder save operation failed due to invalid property values.</m:MessageText>
               <m:ResponseCode>ErrorFolderSavePropertyError</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:MessageXml>
                  <t:FieldURI FieldURI="folder:DisplayName"/>
               </m:MessageXml>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The specified parent folder could not be found.</m:MessageText>
               <m:ResponseCode>ErrorParentFolderNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bb9bf-162">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bb9bf-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb9bf-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="bb9bf-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="bb9bf-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bb9bf-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bb9bf-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bb9bf-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="bb9bf-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="bb9bf-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bb9bf-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bb9bf-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bb9bf-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bb9bf-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="bb9bf-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bb9bf-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="bb9bf-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="bb9bf-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="bb9bf-171">Pastas</span><span class="sxs-lookup"><span data-stu-id="bb9bf-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="bb9bf-172">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="bb9bf-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="bb9bf-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb9bf-173">See also</span></span>

- [<span data-ttu-id="bb9bf-174">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bb9bf-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bb9bf-175">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="bb9bf-175">FindFolder operation</span></span>](findfolder-operation.md)
    

