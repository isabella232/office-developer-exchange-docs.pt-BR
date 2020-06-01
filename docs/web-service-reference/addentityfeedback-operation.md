---
title: Operação AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: A operação AddEntityFeedback retorna informações de erro correspondentes a problemas no servidor.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458436"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="41d32-103">Operação AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="41d32-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="41d32-104">A operação **AddEntityFeedback** retorna informações de erro correspondentes a problemas no servidor.</span><span class="sxs-lookup"><span data-stu-id="41d32-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="41d32-105">Essa operação depende do tipo de evento que está sendo registrado em log.</span><span class="sxs-lookup"><span data-stu-id="41d32-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="41d32-106">Um dos eventos mais importantes é **EntityAdded**, que corresponde a uma entidade que está sendo selecionada.</span><span class="sxs-lookup"><span data-stu-id="41d32-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="41d32-107">Essa operação é em lote, portanto, ela pode ser usada para registrar lotes de entradas em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="41d32-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="41d32-108">Exemplos de solicitação FindPeople</span><span class="sxs-lookup"><span data-stu-id="41d32-108">FindPeople request examples</span></span>

<span data-ttu-id="41d32-109">A operação **AddEntityFeedback** oferece uma maneira de os clientes registrarem detalhes de interação com entidades retornadas pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="41d32-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="41d32-110">Isso pode ser usado como um sinal para melhorar a relevância por trás das cenas para cada cliente.</span><span class="sxs-lookup"><span data-stu-id="41d32-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="41d32-111">Por exemplo, os clientes podem usar essa operação para fornecer comentários sobre entidades de pessoas retornadas de **FindPeople**.</span><span class="sxs-lookup"><span data-stu-id="41d32-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="41d32-112">O conteúdo do corpo SOAP de solicitação</span><span class="sxs-lookup"><span data-stu-id="41d32-112">The request SOAP body contents</span></span>

<span data-ttu-id="41d32-113">A solicitação SOAP contém um único elemento **EntityFeedbackEntries**.</span><span class="sxs-lookup"><span data-stu-id="41d32-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="41d32-114">Isso, por sua vez, contém uma matriz de objetos **EntityFeedbackEntry** .</span><span class="sxs-lookup"><span data-stu-id="41d32-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="41d32-115">Cada entrada na matriz pode conter os seguintes elementos.</span><span class="sxs-lookup"><span data-stu-id="41d32-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="41d32-116">**Parâmetros de solicitação**</span><span class="sxs-lookup"><span data-stu-id="41d32-116">**Request Parameters**</span></span>|<span data-ttu-id="41d32-117">**Obrigatório**</span><span class="sxs-lookup"><span data-stu-id="41d32-117">**Required**</span></span>|<span data-ttu-id="41d32-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41d32-118">**Description**</span></span>|<span data-ttu-id="41d32-119">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="41d32-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="41d32-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="41d32-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="41d32-121">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-121">Yes</span></span>  <br/> |<span data-ttu-id="41d32-122">A hora UTC em que o evento ocorreu no lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="41d32-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="41d32-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="41d32-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="41d32-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="41d32-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="41d32-125">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-125">Yes</span></span>  <br/> |<span data-ttu-id="41d32-126">A hora local em que o evento ocorreu no lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="41d32-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="41d32-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="41d32-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="41d32-128">**ClientId**</span><span class="sxs-lookup"><span data-stu-id="41d32-128">**ClientId**</span></span> <br/> |<span data-ttu-id="41d32-129">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-129">Yes</span></span>  <br/> |<span data-ttu-id="41d32-130">Tipo de cliente (por exemplo, Outlook, OWA, etc.).</span><span class="sxs-lookup"><span data-stu-id="41d32-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="41d32-131">Enumeração ClientIDtype</span><span class="sxs-lookup"><span data-stu-id="41d32-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="41d32-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="41d32-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="41d32-133">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-133">Yes</span></span>  <br/> |<span data-ttu-id="41d32-134">GUID que identifica a ID da sessão.</span><span class="sxs-lookup"><span data-stu-id="41d32-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="41d32-135">Gerado no cliente.</span><span class="sxs-lookup"><span data-stu-id="41d32-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="41d32-136">GUID</span><span class="sxs-lookup"><span data-stu-id="41d32-136">GUID</span></span>  <br/> |
|<span data-ttu-id="41d32-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="41d32-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="41d32-138">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-138">Yes</span></span>  <br/> |<span data-ttu-id="41d32-139">Versão do cliente (por exemplo, 15.01.0101.000).</span><span class="sxs-lookup"><span data-stu-id="41d32-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="41d32-140">String</span><span class="sxs-lookup"><span data-stu-id="41d32-140">String</span></span>  <br/> |
|<span data-ttu-id="41d32-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="41d32-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="41d32-142">Não</span><span class="sxs-lookup"><span data-stu-id="41d32-142">No</span></span>  <br/> |<span data-ttu-id="41d32-143">Fonte para EntityAded (por exemplo, EntityRelevanceAPI, tipos, coladas).</span><span class="sxs-lookup"><span data-stu-id="41d32-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="41d32-144">Enumeração EntityAddSource</span><span class="sxs-lookup"><span data-stu-id="41d32-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="41d32-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="41d32-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="41d32-146">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-146">Yes</span></span>  <br/> |<span data-ttu-id="41d32-147">Um inteiro incremental por sessão de cliente.</span><span class="sxs-lookup"><span data-stu-id="41d32-147">An incremental integer per client session.</span></span> <span data-ttu-id="41d32-148">Usado para detectar a perda de dados.</span><span class="sxs-lookup"><span data-stu-id="41d32-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="41d32-149">Int</span><span class="sxs-lookup"><span data-stu-id="41d32-149">Int</span></span>  <br/> |
|<span data-ttu-id="41d32-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="41d32-150">**EventType**</span></span> <br/> |<span data-ttu-id="41d32-151">Sim</span><span class="sxs-lookup"><span data-stu-id="41d32-151">Yes</span></span>  <br/> |<span data-ttu-id="41d32-152">Tipo de evento (por exemplo, entidade adicionada, entidade removida).</span><span class="sxs-lookup"><span data-stu-id="41d32-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="41d32-153">String</span><span class="sxs-lookup"><span data-stu-id="41d32-153">String</span></span>  <br/> |
|<span data-ttu-id="41d32-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="41d32-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="41d32-155">Não</span><span class="sxs-lookup"><span data-stu-id="41d32-155">No</span></span>  <br/> |<span data-ttu-id="41d32-156">Propriedades adicionais associadas ao evento (blob JSON de pares chave/valor).</span><span class="sxs-lookup"><span data-stu-id="41d32-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="41d32-157">Blob JSON</span><span class="sxs-lookup"><span data-stu-id="41d32-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="41d32-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="41d32-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="41d32-159">Não</span><span class="sxs-lookup"><span data-stu-id="41d32-159">No</span></span>  <br/> |<span data-ttu-id="41d32-160">Lista de entidades associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="41d32-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="41d32-161">Cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="41d32-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="41d32-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="41d32-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="41d32-163">Não</span><span class="sxs-lookup"><span data-stu-id="41d32-163">No</span></span>  <br/> |<span data-ttu-id="41d32-164">ID (GUID) que correlaciona a ID nos logs de consulta.</span><span class="sxs-lookup"><span data-stu-id="41d32-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="41d32-165">String</span><span class="sxs-lookup"><span data-stu-id="41d32-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="41d32-166">Resposta de operação AddEntityFeedback bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="41d32-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="41d32-167">O corpo SOAP de resposta contém os seguintes elementos</span><span class="sxs-lookup"><span data-stu-id="41d32-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="41d32-168">Erros</span><span class="sxs-lookup"><span data-stu-id="41d32-168">Errors</span></span> 
  
<span data-ttu-id="41d32-169">A API pode registrar um lote de entradas de comentários, registramos tudo o que podemos.</span><span class="sxs-lookup"><span data-stu-id="41d32-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="41d32-170">Este campo representa o número de entradas de erro que não foram registradas.</span><span class="sxs-lookup"><span data-stu-id="41d32-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="41d32-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="41d32-171">ErrorDetails</span></span>
  
<span data-ttu-id="41d32-172">Os detalhes referentes aos erros acima são separados por `;` .</span><span class="sxs-lookup"><span data-stu-id="41d32-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="41d32-173">Valores compatíveis no momento</span><span class="sxs-lookup"><span data-stu-id="41d32-173">Currently supported values</span></span>

|<span data-ttu-id="41d32-174">**Enumeração ClientIdtype**</span><span class="sxs-lookup"><span data-stu-id="41d32-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="41d32-175">Desktop</span><span class="sxs-lookup"><span data-stu-id="41d32-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="41d32-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="41d32-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="41d32-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="41d32-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="41d32-178">Lync</span><span class="sxs-lookup"><span data-stu-id="41d32-178">Lync</span></span>  <br/> |
|<span data-ttu-id="41d32-179">, MacMail</span><span class="sxs-lookup"><span data-stu-id="41d32-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="41d32-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="41d32-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="41d32-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="41d32-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="41d32-182">Outros</span><span class="sxs-lookup"><span data-stu-id="41d32-182">Other</span></span>  <br/> |
|<span data-ttu-id="41d32-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="41d32-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="41d32-184">OutlookService</span><span class="sxs-lookup"><span data-stu-id="41d32-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="41d32-185">CORREIO</span><span class="sxs-lookup"><span data-stu-id="41d32-185">POP3</span></span>  <br/> |
|<span data-ttu-id="41d32-186">Tablet</span><span class="sxs-lookup"><span data-stu-id="41d32-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="41d32-187">Web</span><span class="sxs-lookup"><span data-stu-id="41d32-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="41d32-188">**Enumeração EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="41d32-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="41d32-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="41d32-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="41d32-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="41d32-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="41d32-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="41d32-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="41d32-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="41d32-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="41d32-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="41d32-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="41d32-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="41d32-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="41d32-195">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41d32-195">None</span></span>  <br/> |
|<span data-ttu-id="41d32-196">Outros</span><span class="sxs-lookup"><span data-stu-id="41d32-196">Other</span></span>  <br/> |
|<span data-ttu-id="41d32-197">Colar</span><span class="sxs-lookup"><span data-stu-id="41d32-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="41d32-198">Resposta de erro de operação AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="41d32-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="41d32-199">Para códigos de erro genéricos para EWS, confira [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="41d32-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="41d32-200">Exemplo de AddEntityFeedback em conjunto com FindPeople</span><span class="sxs-lookup"><span data-stu-id="41d32-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="41d32-201">Solicitação FindPeople</span><span class="sxs-lookup"><span data-stu-id="41d32-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a><span data-ttu-id="41d32-202">Resposta FindPeople</span><span class="sxs-lookup"><span data-stu-id="41d32-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a><span data-ttu-id="41d32-203">Solicitação AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="41d32-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> <span data-ttu-id="41d32-204">Usando a ID de transação de resposta FindPeople como a ID de transação de solicitação AddEntityFeedback.</span><span class="sxs-lookup"><span data-stu-id="41d32-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="41d32-205">Resposta AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="41d32-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


