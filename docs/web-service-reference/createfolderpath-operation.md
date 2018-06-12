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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751587"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="5b355-103">Operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="5b355-103">CreateFolderPath operation</span></span>

<span data-ttu-id="5b355-104">Encontre informações sobre a operação de EWS **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="5b355-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="5b355-105">A operação **CreateFolderPath** cria uma hierarquia de pastas.</span><span class="sxs-lookup"><span data-stu-id="5b355-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="5b355-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5b355-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="5b355-107">Usando a operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="5b355-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="5b355-108">A solicitação de operação **CreateFolderPath** adota uma matriz de pastas e um identificador de pasta pai e cria uma hierarquia de pastas com base na ordem as pastas na matriz.</span><span class="sxs-lookup"><span data-stu-id="5b355-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="5b355-109">Cabeçalhos SOAP CreateFolderPath operação</span><span class="sxs-lookup"><span data-stu-id="5b355-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="5b355-110">A operação **CreateFolderPath** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5b355-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5b355-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="5b355-111">**Header name**</span></span>|<span data-ttu-id="5b355-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b355-112">**Element**</span></span>|<span data-ttu-id="5b355-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b355-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5b355-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="5b355-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5b355-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5b355-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5b355-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="5b355-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5b355-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b355-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b355-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5b355-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5b355-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5b355-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5b355-120">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5b355-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5b355-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b355-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b355-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5b355-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5b355-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5b355-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5b355-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="5b355-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5b355-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b355-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b355-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5b355-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5b355-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5b355-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5b355-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b355-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5b355-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5b355-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="5b355-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="5b355-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="5b355-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="5b355-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="5b355-132">Identifica o escopo de fuso horário para as propriedades de **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="5b355-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="5b355-133">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b355-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="5b355-134">Exemplo de solicitação de operação CreateFolderPath: criar uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="5b355-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="5b355-135">O exemplo a seguir de uma solicitação de operação **CreateFolderPath** mostra como criar uma hierarquia de pastas é três pastas profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="5b355-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5b355-136">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b355-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="5b355-137">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5b355-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b355-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="5b355-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="5b355-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="5b355-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="5b355-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5b355-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="5b355-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="5b355-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="5b355-142">Folder</span><span class="sxs-lookup"><span data-stu-id="5b355-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5b355-143">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="5b355-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="5b355-144">Resposta de operação CreateFolderPath bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5b355-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="5b355-145">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **CreateFolderPath** para criar uma pasta pastas de hierarquia três profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="5b355-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
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

<span data-ttu-id="5b355-146">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5b355-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b355-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="5b355-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="5b355-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5b355-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5b355-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5b355-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="5b355-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5b355-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5b355-151">Pastas</span><span class="sxs-lookup"><span data-stu-id="5b355-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5b355-152">Folder</span><span class="sxs-lookup"><span data-stu-id="5b355-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5b355-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="5b355-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5b355-154">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="5b355-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5b355-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5b355-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="5b355-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="5b355-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="5b355-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="5b355-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="5b355-158">Resposta de erro de operação CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="5b355-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="5b355-159">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="5b355-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="5b355-160">Esta é uma resposta a uma solicitação para criar duas pastas, a primeira delas não possuem uma propriedade de nome de exibição definido.</span><span class="sxs-lookup"><span data-stu-id="5b355-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="5b355-161">A primeira pasta na hierarquia não pode ser criada sem uma propriedade de nome de exibição e a segunda pasta não pode ser criada porque a pasta pai na hierarquia não foi criada.</span><span class="sxs-lookup"><span data-stu-id="5b355-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
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

<span data-ttu-id="5b355-162">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5b355-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b355-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="5b355-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="5b355-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5b355-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5b355-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5b355-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="5b355-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="5b355-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5b355-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5b355-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5b355-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5b355-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5b355-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5b355-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="5b355-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5b355-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="5b355-171">Pastas</span><span class="sxs-lookup"><span data-stu-id="5b355-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="5b355-172">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5b355-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5b355-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="5b355-173">See also</span></span>

- [<span data-ttu-id="5b355-174">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5b355-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5b355-175">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="5b355-175">FindFolder operation</span></span>](findfolder-operation.md)
    

