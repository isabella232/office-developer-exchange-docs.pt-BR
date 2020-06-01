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
description: A operação FindFolder usa os serviços Web do Exchange para localizar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462581"
---
# <a name="findfolder-operation"></a><span data-ttu-id="af39b-103">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="af39b-103">FindFolder operation</span></span>

<span data-ttu-id="af39b-104">A operação **FindFolder** usa os serviços Web do Exchange para localizar subpastas de uma pasta identificada e retorna um conjunto de propriedades que descrevem o conjunto de subpastas.</span><span class="sxs-lookup"><span data-stu-id="af39b-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="af39b-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="af39b-105">Remarks</span></span>

<span data-ttu-id="af39b-106">FindFolder retorna apenas os primeiros 512 bytes de qualquer propriedade streamable.</span><span class="sxs-lookup"><span data-stu-id="af39b-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="af39b-107">Para Unicode, ele retorna os primeiros 255 caracteres usando uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="af39b-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="af39b-108">Consultas de passagem profunda não podem ser realizadas em pastas públicas.</span><span class="sxs-lookup"><span data-stu-id="af39b-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="af39b-109">As restrições são permitidas e devem usar apenas as propriedades da pasta, não as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="af39b-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="af39b-110">A funcionalidade de classificação não está disponível para respostas **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="af39b-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="af39b-111">As consultas agrupadas não estão disponíveis para consultas do **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="af39b-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="af39b-112">**Observação** A operação **FindFolder** também é usada para localizar pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="af39b-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="af39b-113">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="af39b-113">SOAP Headers</span></span>

<span data-ttu-id="af39b-114">A operação **FindFolder** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="af39b-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="af39b-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="af39b-115">**Header**</span></span>|<span data-ttu-id="af39b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af39b-116">**Element**</span></span>|<span data-ttu-id="af39b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af39b-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="af39b-118">Representação</span><span class="sxs-lookup"><span data-stu-id="af39b-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="af39b-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="af39b-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="af39b-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="af39b-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="af39b-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="af39b-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="af39b-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="af39b-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="af39b-123">Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="af39b-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="af39b-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="af39b-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="af39b-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="af39b-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="af39b-126">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="af39b-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="af39b-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="af39b-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="af39b-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="af39b-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="af39b-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="af39b-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="af39b-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="af39b-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="af39b-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="af39b-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="af39b-132">Identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="af39b-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="af39b-133">Exemplo de solicitação FindFolder</span><span class="sxs-lookup"><span data-stu-id="af39b-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="af39b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="af39b-134">Description</span></span>

<span data-ttu-id="af39b-135">O exemplo a seguir de uma solicitação **FindFolder** mostra como formar uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="af39b-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="af39b-136">Código</span><span class="sxs-lookup"><span data-stu-id="af39b-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="af39b-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="af39b-137">Comments</span></span>

<span data-ttu-id="af39b-138">Usando o valor padrão para o [BaseShape](baseshape.md), a resposta retorna o nome da pasta, a ID da pasta, o número de subpastas, o número de pastas filhas encontradas na pasta e a contagem de itens não lidos.</span><span class="sxs-lookup"><span data-stu-id="af39b-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="af39b-139">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="af39b-139">Request elements</span></span>

<span data-ttu-id="af39b-140">Essa solicitação de **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="af39b-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="af39b-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="af39b-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="af39b-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="af39b-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="af39b-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="af39b-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="af39b-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="af39b-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="af39b-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="af39b-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="af39b-146">Para obter outros elementos de solicitação do **FindFolder** , consulte o esquema.</span><span class="sxs-lookup"><span data-stu-id="af39b-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="af39b-147">Exemplo de resposta FindFolder</span><span class="sxs-lookup"><span data-stu-id="af39b-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="af39b-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="af39b-148">Description</span></span>

<span data-ttu-id="af39b-149">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida à solicitação **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="af39b-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="af39b-150">A resposta contém os elementos que são retornados quando o valor padrão para [BaseShape](baseshape.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="af39b-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="af39b-151">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af39b-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="af39b-152">Código</span><span class="sxs-lookup"><span data-stu-id="af39b-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="af39b-153">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="af39b-153">Response elements</span></span>

<span data-ttu-id="af39b-154">As propriedades que são retornadas na resposta são determinadas pelo [BaseShape](baseshape.md) e asproperties [adicionais](additionalproperties.md) se forem usadas.</span><span class="sxs-lookup"><span data-stu-id="af39b-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="af39b-155">Uma resposta bem-sucedida do **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="af39b-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="af39b-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="af39b-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="af39b-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="af39b-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="af39b-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="af39b-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="af39b-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="af39b-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="af39b-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="af39b-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="af39b-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="af39b-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="af39b-162">Pastas</span><span class="sxs-lookup"><span data-stu-id="af39b-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="af39b-163">Folder</span><span class="sxs-lookup"><span data-stu-id="af39b-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="af39b-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="af39b-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="af39b-165">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="af39b-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="af39b-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="af39b-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="af39b-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="af39b-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="af39b-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="af39b-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="af39b-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="af39b-169">Comments</span></span>

 <span data-ttu-id="af39b-170">As respostas **FindFolder** a uma solicitação com a forma de resposta **myproperties** não retornarão os elementos [TotalCount](totalcount.md) e [UnreadCount](unreadcount.md) para pesquisas de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="af39b-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="af39b-171">Exemplo de resposta de erro FindFolder</span><span class="sxs-lookup"><span data-stu-id="af39b-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="af39b-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="af39b-172">Description</span></span>

<span data-ttu-id="af39b-173">O seguinte exemplo de corpo SOAP mostra uma resposta de erro que ocorre quando você procura uma pasta identificada por um identificador de pasta malformado.</span><span class="sxs-lookup"><span data-stu-id="af39b-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="af39b-174">Código</span><span class="sxs-lookup"><span data-stu-id="af39b-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="af39b-175">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="af39b-175">Error response elements</span></span>

<span data-ttu-id="af39b-176">A resposta de erro **FindFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="af39b-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="af39b-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="af39b-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="af39b-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="af39b-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="af39b-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="af39b-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="af39b-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="af39b-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="af39b-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="af39b-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="af39b-182">Informações Adicionais</span><span class="sxs-lookup"><span data-stu-id="af39b-182">Additional Information</span></span>

- <span data-ttu-id="af39b-183">O elemento [DisplayName (cadeia de caracteres)](displayname-string.md) da pasta sempre é incluído na forma padrão.</span><span class="sxs-lookup"><span data-stu-id="af39b-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="af39b-184">O elemento [UnreadCount](unreadcount.md) está incluído nas pastas tarefas e anotações.</span><span class="sxs-lookup"><span data-stu-id="af39b-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="af39b-185">Use o valor **PropertyTag** de 0x672D com um tipo de propriedade de **inteiro** para identificar uma pasta gerenciada usando o elemento [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="af39b-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="af39b-186">Também consulte</span><span class="sxs-lookup"><span data-stu-id="af39b-186">See also</span></span>



[<span data-ttu-id="af39b-187">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="af39b-187">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

