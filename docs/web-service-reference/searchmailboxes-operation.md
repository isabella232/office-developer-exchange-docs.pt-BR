---
title: Operação SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Encontre informações sobre o EWS SearchMailboxes operação.
ms.openlocfilehash: 141ea466a24f3cb400a8e0b63e2162c1eae5d7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825296"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="0c19c-103">Operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-103">SearchMailboxes operation</span></span>

<span data-ttu-id="0c19c-104">Encontre informações sobre a operação de EWS **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="0c19c-104">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="0c19c-105">A operação **SearchMailboxes** procura por caixas de correio de ocorrências de termos em itens da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c19c-105">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="0c19c-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0c19c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="0c19c-107">Usando a operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-107">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="0c19c-108">A operação **SearchMailboxes** pode usar muitas consultas de pesquisa simultâneas para executar a pesquisa de descoberta em várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="0c19c-108">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="0c19c-109">Os resultados podem ser qualquer um dos informações estatísticas sobre o número de vezes que ocorrem de termos de pesquisa ou uma visualização dos itens que contenham os termos de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0c19c-109">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="0c19c-110">Cabeçalhos SOAP SearchMailboxes operação</span><span class="sxs-lookup"><span data-stu-id="0c19c-110">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="0c19c-111">A operação **SearchMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0c19c-111">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0c19c-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="0c19c-112">**Header name**</span></span>|<span data-ttu-id="0c19c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c19c-113">**Element**</span></span>|<span data-ttu-id="0c19c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c19c-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0c19c-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="0c19c-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="0c19c-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="0c19c-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="0c19c-117">Identifica as funções de servidor necessários para que o chamador para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c19c-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="0c19c-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c19c-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c19c-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0c19c-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0c19c-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0c19c-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0c19c-121">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="0c19c-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0c19c-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c19c-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0c19c-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0c19c-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0c19c-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0c19c-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0c19c-125">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c19c-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0c19c-126">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0c19c-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="0c19c-127">Exemplo de solicitação de operação SearchMailboxes: caixas de correio para o número de ocorrências de pesquisa de termos de pesquisa</span><span class="sxs-lookup"><span data-stu-id="0c19c-127">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="0c19c-128">O exemplo a seguir de uma solicitação de operação **SearchMailboxes** mostra como usar dois diferentes consultas para pesquisar três caixas de correio diferentes para informações estatísticas sobre quantas vezes um termo aparece em cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c19c-128">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0c19c-129">Neste exemplo, o elemento de [consulta](query.md) é intentionaly deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="0c19c-129">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="0c19c-130">É exibida como uma solicitação bem-sucedida pode conter condições de erro em um por base de pesquisa de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c19c-130">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="0c19c-131">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0c19c-131">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c19c-132">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-132">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="0c19c-133">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="0c19c-133">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="0c19c-134">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="0c19c-134">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="0c19c-135">Query</span><span class="sxs-lookup"><span data-stu-id="0c19c-135">Query</span></span>](query.md)
    
- [<span data-ttu-id="0c19c-136">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="0c19c-136">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="0c19c-137">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-137">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="0c19c-138">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="0c19c-138">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0c19c-139">SearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-139">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="0c19c-140">ResultType</span><span class="sxs-lookup"><span data-stu-id="0c19c-140">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="0c19c-141">Resposta de operação SearchMailboxes bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0c19c-141">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="0c19c-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SearchMailboxes** para obter informações estatísticas sobre o número de vezes que os termos de pesquisa são encontrados nas caixas de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="0c19c-142">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="0c19c-143">A última consulta contém um elemento vazio de **consulta** , que mostra uma pesquisa de caixa de correio com falha.</span><span class="sxs-lookup"><span data-stu-id="0c19c-143">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="0c19c-144">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0c19c-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c19c-145">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="0c19c-145">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="0c19c-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0c19c-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0c19c-147">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0c19c-147">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="0c19c-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c19c-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c19c-149">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="0c19c-149">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="0c19c-150">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="0c19c-150">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="0c19c-151">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="0c19c-151">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="0c19c-152">Query</span><span class="sxs-lookup"><span data-stu-id="0c19c-152">Query</span></span>](query.md)
    
- [<span data-ttu-id="0c19c-153">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="0c19c-153">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="0c19c-154">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-154">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="0c19c-155">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="0c19c-155">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0c19c-156">SearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-156">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="0c19c-157">ResultType</span><span class="sxs-lookup"><span data-stu-id="0c19c-157">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="0c19c-158">ItemCount</span><span class="sxs-lookup"><span data-stu-id="0c19c-158">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="0c19c-159">Tamanho (long)</span><span class="sxs-lookup"><span data-stu-id="0c19c-159">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="0c19c-160">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="0c19c-160">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="0c19c-161">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="0c19c-161">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="0c19c-162">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="0c19c-162">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="0c19c-163">Palavra-chave</span><span class="sxs-lookup"><span data-stu-id="0c19c-163">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="0c19c-164">ItemHits</span><span class="sxs-lookup"><span data-stu-id="0c19c-164">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="0c19c-165">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-165">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="0c19c-166">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="0c19c-166">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="0c19c-167">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="0c19c-167">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0c19c-168">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="0c19c-168">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="0c19c-169">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="0c19c-169">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="0c19c-170">IsArchive</span><span class="sxs-lookup"><span data-stu-id="0c19c-170">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="0c19c-171">Resposta de erro de operação SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-171">SearchMailboxes operation error response</span></span>

<span data-ttu-id="0c19c-172">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="0c19c-172">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="0c19c-173">Esta é uma resposta a uma solicitação para pesquisar uma caixa de correio quando o identificador de caixa de correio está incorreto.</span><span class="sxs-lookup"><span data-stu-id="0c19c-173">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="0c19c-174">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0c19c-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0c19c-175">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="0c19c-175">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="0c19c-176">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0c19c-176">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0c19c-177">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0c19c-177">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="0c19c-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0c19c-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0c19c-179">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="0c19c-179">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="0c19c-180">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="0c19c-180">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="0c19c-181">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="0c19c-181">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="0c19c-182">Query</span><span class="sxs-lookup"><span data-stu-id="0c19c-182">Query</span></span>](query.md)
    
- [<span data-ttu-id="0c19c-183">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="0c19c-183">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="0c19c-184">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-184">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="0c19c-185">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="0c19c-185">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0c19c-186">SearchScope</span><span class="sxs-lookup"><span data-stu-id="0c19c-186">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="0c19c-187">ResultType</span><span class="sxs-lookup"><span data-stu-id="0c19c-187">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="0c19c-188">ItemCount</span><span class="sxs-lookup"><span data-stu-id="0c19c-188">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="0c19c-189">Tamanho (long)</span><span class="sxs-lookup"><span data-stu-id="0c19c-189">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="0c19c-190">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="0c19c-190">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="0c19c-191">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="0c19c-191">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="0c19c-192">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-192">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="0c19c-193">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="0c19c-193">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="0c19c-194">Caixa de correio (string)</span><span class="sxs-lookup"><span data-stu-id="0c19c-194">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="0c19c-195">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="0c19c-195">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="0c19c-196">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="0c19c-196">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="0c19c-197">IsArchive</span><span class="sxs-lookup"><span data-stu-id="0c19c-197">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="0c19c-198">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="0c19c-198">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0c19c-199">Confira também</span><span class="sxs-lookup"><span data-stu-id="0c19c-199">See also</span></span>

- [<span data-ttu-id="0c19c-200">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c19c-200">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0c19c-201">Operação GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-201">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="0c19c-202">Operação SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-202">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="0c19c-203">Operação GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0c19c-203">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="0c19c-204">Operação GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c19c-204">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="0c19c-205">Operação GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="0c19c-205">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="0c19c-206">Operação GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="0c19c-206">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

