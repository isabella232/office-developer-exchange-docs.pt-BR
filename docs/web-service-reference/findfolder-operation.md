---
title: Operação FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: A operação FindFolder usa serviços Web do Exchange para localizar as subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752270"
---
# <a name="findfolder-operation"></a><span data-ttu-id="52b01-103">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="52b01-103">FindFolder operation</span></span>

<span data-ttu-id="52b01-104">A operação **FindFolder** usa serviços Web do Exchange para localizar as subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.</span><span class="sxs-lookup"><span data-stu-id="52b01-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="52b01-105">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="52b01-105">Remarks</span></span>

<span data-ttu-id="52b01-106">FindFolder retorna apenas os primeiros 512 bytes de qualquer propriedade transmissíveis.</span><span class="sxs-lookup"><span data-stu-id="52b01-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="52b01-107">Para Unicode, ele retorna os primeiros 255 caracteres, usando uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="52b01-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="52b01-108">Consultas percurso profundo não podem ser executadas em pastas públicas.</span><span class="sxs-lookup"><span data-stu-id="52b01-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="52b01-109">Restrições são permitidas e devem usar apenas as propriedades de pasta, não as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="52b01-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="52b01-110">Classificar funcionalidade não está disponível para **FindFolder** respostas.</span><span class="sxs-lookup"><span data-stu-id="52b01-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="52b01-111">Consultas agrupadas não estão disponíveis para consultas **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="52b01-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="52b01-112">**Observação** A operação **FindFolder** também é usada para localizar pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="52b01-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="52b01-113">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="52b01-113">SOAP Headers</span></span>

<span data-ttu-id="52b01-114">A operação **FindFolder** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="52b01-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="52b01-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="52b01-115">**Header**</span></span>|<span data-ttu-id="52b01-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="52b01-116">**Element**</span></span>|<span data-ttu-id="52b01-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52b01-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52b01-118">Representação</span><span class="sxs-lookup"><span data-stu-id="52b01-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="52b01-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="52b01-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="52b01-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="52b01-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="52b01-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="52b01-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="52b01-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="52b01-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="52b01-123">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52b01-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="52b01-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="52b01-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="52b01-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="52b01-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="52b01-126">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="52b01-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="52b01-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="52b01-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="52b01-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="52b01-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="52b01-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="52b01-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="52b01-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="52b01-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="52b01-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="52b01-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="52b01-132">Identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="52b01-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="52b01-133">Exemplo de solicitação FindFolder</span><span class="sxs-lookup"><span data-stu-id="52b01-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="52b01-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b01-134">Description</span></span>

<span data-ttu-id="52b01-135">O exemplo a seguir de uma solicitação de **FindFolder** mostra como uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada de formulário.</span><span class="sxs-lookup"><span data-stu-id="52b01-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="52b01-136">Código</span><span class="sxs-lookup"><span data-stu-id="52b01-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="52b01-137">Comments</span><span class="sxs-lookup"><span data-stu-id="52b01-137">Comments</span></span>

<span data-ttu-id="52b01-138">Usando o valor padrão para o [BaseShape](baseshape.md), a resposta retorna o nome da pasta, o ID de pasta, o número de subpastas, o número de pastas filho encontrado na pasta e a contagem de itens não lidos.</span><span class="sxs-lookup"><span data-stu-id="52b01-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="52b01-139">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52b01-139">Request elements</span></span>

<span data-ttu-id="52b01-140">Essa solicitação **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="52b01-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="52b01-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="52b01-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="52b01-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="52b01-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="52b01-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="52b01-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="52b01-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="52b01-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="52b01-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="52b01-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="52b01-146">Para elementos de solicitação **FindFolder** adicionais, consulte o esquema.</span><span class="sxs-lookup"><span data-stu-id="52b01-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="52b01-147">Exemplo de resposta FindFolder</span><span class="sxs-lookup"><span data-stu-id="52b01-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="52b01-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b01-148">Description</span></span>

<span data-ttu-id="52b01-149">O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="52b01-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="52b01-150">A resposta conterá os elementos que são retornados quando o valor padrão para o [BaseShape](baseshape.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="52b01-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="52b01-151">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52b01-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="52b01-152">Código</span><span class="sxs-lookup"><span data-stu-id="52b01-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="52b01-153">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="52b01-153">Response elements</span></span>

<span data-ttu-id="52b01-154">As propriedades que são retornadas na resposta são determinadas pelo [BaseShape](baseshape.md) e o [AdditionalProperties](additionalproperties.md) se eles são usados.</span><span class="sxs-lookup"><span data-stu-id="52b01-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="52b01-155">Uma resposta bem-sucedida do **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="52b01-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="52b01-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="52b01-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="52b01-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="52b01-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="52b01-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="52b01-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="52b01-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="52b01-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="52b01-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="52b01-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="52b01-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="52b01-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="52b01-162">Pastas</span><span class="sxs-lookup"><span data-stu-id="52b01-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="52b01-163">Folder</span><span class="sxs-lookup"><span data-stu-id="52b01-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="52b01-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="52b01-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="52b01-165">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="52b01-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="52b01-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="52b01-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="52b01-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="52b01-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="52b01-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="52b01-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="52b01-169">Comments</span><span class="sxs-lookup"><span data-stu-id="52b01-169">Comments</span></span>

 <span data-ttu-id="52b01-170">Respostas **FindFolder** a uma solicitação com a forma de resposta **AllProperties** não retornará o [TotalCount](totalcount.md) e os elementos de [UnreadCount](unreadcount.md) para pesquisas de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="52b01-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="52b01-171">Exemplo de resposta de erro FindFolder</span><span class="sxs-lookup"><span data-stu-id="52b01-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="52b01-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b01-172">Description</span></span>

<span data-ttu-id="52b01-173">O exemplo de corpo SOAP a seguir mostra uma resposta de erro que ocorre quando você procurar uma pasta que é identificada por um identificador de pasta mal formados.</span><span class="sxs-lookup"><span data-stu-id="52b01-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="52b01-174">Código</span><span class="sxs-lookup"><span data-stu-id="52b01-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="52b01-175">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="52b01-175">Error response elements</span></span>

<span data-ttu-id="52b01-176">A resposta de erro **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="52b01-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="52b01-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="52b01-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="52b01-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="52b01-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="52b01-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="52b01-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="52b01-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="52b01-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="52b01-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="52b01-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="52b01-182">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="52b01-182">Additional Information</span></span>

- <span data-ttu-id="52b01-183">O elemento de [DisplayName (string)](displayname-string.md) da pasta é sempre incluído na forma padrão.</span><span class="sxs-lookup"><span data-stu-id="52b01-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="52b01-184">O elemento [UnreadCount](unreadcount.md) está incluído nas pastas de tarefas e anotações.</span><span class="sxs-lookup"><span data-stu-id="52b01-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="52b01-185">Use o valor **PropertyTag não** 0x672D com um tipo de propriedade de **inteiro** para identificar uma pasta gerenciada usando o elemento [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="52b01-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="52b01-186">Confira também</span><span class="sxs-lookup"><span data-stu-id="52b01-186">See also</span></span>



[<span data-ttu-id="52b01-187">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="52b01-187">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

