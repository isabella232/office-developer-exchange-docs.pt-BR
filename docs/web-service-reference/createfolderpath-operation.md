---
title: Operação createfolderpath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: Encontre informações sobre a operação do EWS de createfolderpath.
ms.openlocfilehash: a8d42cbef854d900c5fb6b72c730dd1e2b903aec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458898"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="1d528-103">Operação createfolderpath</span><span class="sxs-lookup"><span data-stu-id="1d528-103">CreateFolderPath operation</span></span>

<span data-ttu-id="1d528-104">Encontre informações sobre a operação do EWS de **createfolderpath** .</span><span class="sxs-lookup"><span data-stu-id="1d528-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="1d528-105">A operação **createfolderpath** cria uma hierarquia de pastas.</span><span class="sxs-lookup"><span data-stu-id="1d528-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="1d528-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1d528-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="1d528-107">Usando a operação createfolderpath</span><span class="sxs-lookup"><span data-stu-id="1d528-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="1d528-108">A solicitação de operação **createfolderpath** usa uma matriz de pastas e um identificador de pasta pai e cria uma hierarquia de pastas com base na ordem das pastas na matriz.</span><span class="sxs-lookup"><span data-stu-id="1d528-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="1d528-109">Cabeçalhos SOAP de operação createfolderpath</span><span class="sxs-lookup"><span data-stu-id="1d528-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="1d528-110">A operação **createfolderpath** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1d528-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1d528-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="1d528-111">**Header name**</span></span>|<span data-ttu-id="1d528-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1d528-112">**Element**</span></span>|<span data-ttu-id="1d528-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1d528-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1d528-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="1d528-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1d528-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1d528-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1d528-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="1d528-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1d528-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d528-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1d528-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1d528-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1d528-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1d528-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1d528-120">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1d528-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1d528-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d528-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1d528-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1d528-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1d528-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1d528-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1d528-124">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="1d528-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1d528-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d528-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1d528-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1d528-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1d528-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1d528-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1d528-128">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d528-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1d528-129">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="1d528-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="1d528-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="1d528-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="1d528-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="1d528-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="1d528-132">Identifica o escopo de fuso horário para as propriedades **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="1d528-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="1d528-133">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d528-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="1d528-134">Exemplo de solicitação de operação createfolderpath: criar uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="1d528-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="1d528-135">O exemplo a seguir de uma solicitação de operação **createfolderpath** mostra como criar uma hierarquia de pastas que tenha três pastas em profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="1d528-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1d528-136">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d528-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="1d528-137">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="1d528-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1d528-138">Createfolderpath</span><span class="sxs-lookup"><span data-stu-id="1d528-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="1d528-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="1d528-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="1d528-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="1d528-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="1d528-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="1d528-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="1d528-142">Folder</span><span class="sxs-lookup"><span data-stu-id="1d528-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1d528-143">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="1d528-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="1d528-144">Resposta de operação createfolderpath bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="1d528-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="1d528-145">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **createfolderpath** para criar uma hierarquia de pastas três pastas de profundidade na pasta de caixa de entrada padrão.</span><span class="sxs-lookup"><span data-stu-id="1d528-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="1d528-146">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="1d528-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1d528-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="1d528-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="1d528-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d528-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1d528-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d528-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="1d528-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d528-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1d528-151">Pastas</span><span class="sxs-lookup"><span data-stu-id="1d528-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="1d528-152">Folder</span><span class="sxs-lookup"><span data-stu-id="1d528-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="1d528-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="1d528-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="1d528-154">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="1d528-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1d528-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1d528-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="1d528-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="1d528-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="1d528-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="1d528-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="1d528-158">Resposta de erro de operação createfolderpath</span><span class="sxs-lookup"><span data-stu-id="1d528-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="1d528-159">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **createfolderpath** .</span><span class="sxs-lookup"><span data-stu-id="1d528-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="1d528-160">Esta é uma resposta a uma solicitação para criar duas pastas, a primeira que não tem uma propriedade de nome de exibição definida.</span><span class="sxs-lookup"><span data-stu-id="1d528-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="1d528-161">A primeira pasta na hierarquia não pode ser criada sem uma propriedade de nome para exibição, e não é possível criar a segunda pasta porque a pasta pai na hierarquia não foi criada.</span><span class="sxs-lookup"><span data-stu-id="1d528-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="1d528-162">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="1d528-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1d528-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="1d528-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="1d528-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d528-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1d528-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d528-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="1d528-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="1d528-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1d528-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d528-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1d528-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1d528-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1d528-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1d528-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="1d528-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1d528-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="1d528-171">Pastas</span><span class="sxs-lookup"><span data-stu-id="1d528-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="1d528-172">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="1d528-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1d528-173">Também consulte</span><span class="sxs-lookup"><span data-stu-id="1d528-173">See also</span></span>

- [<span data-ttu-id="1d528-174">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1d528-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="1d528-175">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="1d528-175">FindFolder operation</span></span>](findfolder-operation.md)
    

