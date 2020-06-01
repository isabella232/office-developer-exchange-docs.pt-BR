---
title: Operação SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Encontre informações sobre a operação do EWS do SearchMailboxes.
ms.openlocfilehash: 9ec7e9dd4ef17f22f236e64ca1fdbeb65e6e56fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456721"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="73030-103">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-103">SearchMailboxes operation</span></span>

> [!NOTE]
> <span data-ttu-id="73030-104">Essa operação foi preterida e não tem mais suporte da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="73030-104">This operation is deprecated, and no longer supported by Microsoft.</span></span>  <span data-ttu-id="73030-105">Como substituição, use a operação [FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="73030-105">As a replacement, please use the [FindItem](finditem-operation.md) operation.</span></span>

<span data-ttu-id="73030-106">Encontre informações sobre a operação do EWS do **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="73030-106">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="73030-107">A operação **SearchMailboxes** pesquisa caixas de correio para ocorrências de termos em itens de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73030-107">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="73030-108">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73030-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="73030-109">Usando a operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-109">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="73030-110">A operação **SearchMailboxes** pode usar muitas consultas de pesquisa simultâneas para executar a pesquisa de descoberta em várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="73030-110">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="73030-111">Os resultados podem ser informações estatísticas sobre o número de vezes que os termos de pesquisa ocorrem ou uma visualização dos itens que contêm os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="73030-111">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="73030-112">Cabeçalhos SOAP de operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-112">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="73030-113">A operação **SearchMailboxes** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="73030-113">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="73030-114">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="73030-114">**Header name**</span></span>|<span data-ttu-id="73030-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="73030-115">**Element**</span></span>|<span data-ttu-id="73030-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="73030-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73030-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="73030-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="73030-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="73030-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="73030-119">Identifica as funções de servidor necessárias para que o chamador faça a solicitação.</span><span class="sxs-lookup"><span data-stu-id="73030-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="73030-120">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="73030-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73030-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="73030-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="73030-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="73030-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="73030-123">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="73030-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="73030-124">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="73030-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73030-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="73030-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="73030-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="73030-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="73030-127">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="73030-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="73030-128">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="73030-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="73030-129">Exemplo de solicitação de operação SearchMailboxes: Pesquisar caixas de correio para o número de acertos de termos de pesquisa</span><span class="sxs-lookup"><span data-stu-id="73030-129">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="73030-130">O exemplo a seguir de uma solicitação de operação **SearchMailboxes** mostra como usar duas consultas diferentes para pesquisar três caixas de correio diferentes para obter informações estatísticas sobre quantas vezes um termo aparece em cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73030-130">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="73030-131">Neste exemplo, o elemento de [consulta](query.md) é intencionalmente deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="73030-131">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="73030-132">Isso mostra como uma solicitação bem-sucedida pode conter condições de erro em uma base de pesquisa por caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73030-132">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SearchMailboxes>
         <m:SearchQueries>
            <t:MailboxQuery>
               <t:Query>Test Item</t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=12311a742f0e47e392c8201a60d13ecf-Steve</t:Mailbox>
                     <t:SearchScope>All</t:SearchScope>
                  </t:MailboxSearchScope>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=f00c9f70539844beb52341d8f40c572e-Antho</t:Mailbox>
                     <t:SearchScope>PrimaryOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
            <t:MailboxQuery>
               <t:Query></t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=accba4fd5ddf12214a0e82ce1645f4e-Danie</t:Mailbox>
                     <t:SearchScope>ArchiveOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
         </m:SearchQueries>
         <m:ResultType>StatisticsOnly</m:ResultType>
      </m:SearchMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="73030-133">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="73030-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73030-134">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-134">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="73030-135">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="73030-135">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="73030-136">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="73030-136">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="73030-137">Query</span><span class="sxs-lookup"><span data-stu-id="73030-137">Query</span></span>](query.md)
    
- [<span data-ttu-id="73030-138">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="73030-138">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="73030-139">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-139">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="73030-140">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="73030-140">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="73030-141">SearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-141">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="73030-142">ResultType</span><span class="sxs-lookup"><span data-stu-id="73030-142">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="73030-143">Resposta de operação SearchMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="73030-143">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="73030-144">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SearchMailboxes** para obter informações estatísticas sobre o número de vezes que os termos de pesquisa são encontrados nas caixas de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="73030-144">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="73030-145">A última consulta contém um elemento de **consulta** vazio, que mostra uma pesquisa de caixa de correio com falha.</span><span class="sxs-lookup"><span data-stu-id="73030-145">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=35181a94327e392c8201a60d13ecf-Steve</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=f00c9f789572-beb04001d8f40c572e-Antho</t:Mailbox>
                              <t:SearchScope>PrimaryOnly</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>2</t:ItemCount>
                  <t:Size>20206</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:KeywordStats>
                     <t:KeywordStat>
                        <t:Keyword>Test Item</t:Keyword>
                        <t:ItemHits>2</t:ItemHits>
                        <t:Size>20206</t:Size>
                     </t:KeywordStat>
                  </t:KeywordStats>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=accba4as3df234234a0e82ce1645f4e-Danie</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>The search query can't be empty.</t:ErrorMessage>
                        <t:IsArchive>true</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="73030-146">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="73030-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73030-147">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="73030-147">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="73030-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="73030-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="73030-149">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73030-149">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="73030-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="73030-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="73030-151">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="73030-151">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="73030-152">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="73030-152">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="73030-153">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="73030-153">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="73030-154">Query</span><span class="sxs-lookup"><span data-stu-id="73030-154">Query</span></span>](query.md)
    
- [<span data-ttu-id="73030-155">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="73030-155">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="73030-156">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-156">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="73030-157">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="73030-157">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="73030-158">SearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-158">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="73030-159">ResultType</span><span class="sxs-lookup"><span data-stu-id="73030-159">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="73030-160">ItemCount</span><span class="sxs-lookup"><span data-stu-id="73030-160">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="73030-161">Tamanho (longo)</span><span class="sxs-lookup"><span data-stu-id="73030-161">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="73030-162">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="73030-162">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="73030-163">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="73030-163">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="73030-164">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="73030-164">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="73030-165">Chaves</span><span class="sxs-lookup"><span data-stu-id="73030-165">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="73030-166">Hits</span><span class="sxs-lookup"><span data-stu-id="73030-166">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="73030-167">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-167">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="73030-168">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="73030-168">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="73030-169">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="73030-169">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="73030-170">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="73030-170">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="73030-171">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="73030-171">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="73030-172">IsArchive</span><span class="sxs-lookup"><span data-stu-id="73030-172">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="73030-173">Resposta de erro de operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-173">SearchMailboxes operation error response</span></span>

<span data-ttu-id="73030-174">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="73030-174">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="73030-175">Esta é uma resposta a uma solicitação de pesquisa de uma caixa de correio quando o identificador de caixa de correio está incorreto.</span><span class="sxs-lookup"><span data-stu-id="73030-175">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Error">
               <m:MessageText>No mailbox is specified for search operation. If specified in the request, 
               then it could be due to permission issue.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>subject:Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>0</t:ItemCount>
                  <t:Size>0</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>No mailbox is specified for search operation. If specified in the request, 
                        then it could be due to permission issue.</t:ErrorMessage>
                        <t:IsArchive>false</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="73030-176">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="73030-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73030-177">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="73030-177">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="73030-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="73030-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="73030-179">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73030-179">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="73030-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="73030-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="73030-181">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="73030-181">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="73030-182">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="73030-182">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="73030-183">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="73030-183">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="73030-184">Query</span><span class="sxs-lookup"><span data-stu-id="73030-184">Query</span></span>](query.md)
    
- [<span data-ttu-id="73030-185">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="73030-185">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="73030-186">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-186">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="73030-187">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="73030-187">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="73030-188">SearchScope</span><span class="sxs-lookup"><span data-stu-id="73030-188">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="73030-189">ResultType</span><span class="sxs-lookup"><span data-stu-id="73030-189">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="73030-190">ItemCount</span><span class="sxs-lookup"><span data-stu-id="73030-190">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="73030-191">Tamanho (longo)</span><span class="sxs-lookup"><span data-stu-id="73030-191">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="73030-192">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="73030-192">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="73030-193">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="73030-193">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="73030-194">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-194">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="73030-195">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="73030-195">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="73030-196">Caixa de correio (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="73030-196">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="73030-197">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="73030-197">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="73030-198">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="73030-198">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="73030-199">IsArchive</span><span class="sxs-lookup"><span data-stu-id="73030-199">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="73030-200">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="73030-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="73030-201">Também consulte</span><span class="sxs-lookup"><span data-stu-id="73030-201">See also</span></span>

- [<span data-ttu-id="73030-202">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="73030-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="73030-203">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-203">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="73030-204">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-204">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="73030-205">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="73030-205">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="73030-206">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="73030-206">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="73030-207">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="73030-207">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="73030-208">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="73030-208">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

