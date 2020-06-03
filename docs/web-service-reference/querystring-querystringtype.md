---
title: QueryString (QueryStringtype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: O elemento QueryString contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459185"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="a0e36-103">QueryString (QueryStringtype)</span><span class="sxs-lookup"><span data-stu-id="a0e36-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="a0e36-104">O elemento **QueryString** contém uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).</span><span class="sxs-lookup"><span data-stu-id="a0e36-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="a0e36-105">**QueryStringtype**</span><span class="sxs-lookup"><span data-stu-id="a0e36-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0e36-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a0e36-106">Attributes and elements</span></span>

<span data-ttu-id="a0e36-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0e36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0e36-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0e36-108">Attributes</span></span>

|<span data-ttu-id="a0e36-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a0e36-109">**Attribute**</span></span>|<span data-ttu-id="a0e36-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0e36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0e36-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="a0e36-111">ResetCache</span></span>  <br/> |<span data-ttu-id="a0e36-112">Indica que o cache deve ser redefinido.</span><span class="sxs-lookup"><span data-stu-id="a0e36-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="a0e36-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="a0e36-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="a0e36-114">Indica que os itens excluídos devem ser retornados.</span><span class="sxs-lookup"><span data-stu-id="a0e36-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="a0e36-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="a0e36-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="a0e36-116">Indica que os termos realçados devem ser retornados.</span><span class="sxs-lookup"><span data-stu-id="a0e36-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0e36-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0e36-117">Child elements</span></span>

<span data-ttu-id="a0e36-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0e36-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0e36-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0e36-119">Parent elements</span></span>

|<span data-ttu-id="a0e36-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0e36-120">**Element**</span></span>|<span data-ttu-id="a0e36-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0e36-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0e36-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="a0e36-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="a0e36-123">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a0e36-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="a0e36-124">A seguir está a expressão XPath para este elemento:/FindItem.</span><span class="sxs-lookup"><span data-stu-id="a0e36-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0e36-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a0e36-125">Text value</span></span>

<span data-ttu-id="a0e36-126">O valor de texto do elemento **QueryString** representa uma consulta de caixa de correio que é feita usando um subconjunto de [sintaxe de consulta avançada (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a0e36-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="a0e36-127">Consulte a seção comentários para obter informações sobre as opções de sintaxe suportadas para cadeias de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="a0e36-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0e36-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0e36-128">Remarks</span></span>

<span data-ttu-id="a0e36-129">No Exchange Server 2010, esse elemento é um tipo de cadeia de caracteres de esquema XML.</span><span class="sxs-lookup"><span data-stu-id="a0e36-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="a0e36-130">Nas versões do Exchange a partir do Exchange Server 2013, incluindo o Exchange Online, o tipo desse elemento é **querystringtype**.</span><span class="sxs-lookup"><span data-stu-id="a0e36-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="a0e36-131">Essa alteração não quebra clientes existentes porque adiciona três novos atributos opcionais.</span><span class="sxs-lookup"><span data-stu-id="a0e36-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="a0e36-132">O elemento **QueryString** exclui o uso de restrições do EWS.</span><span class="sxs-lookup"><span data-stu-id="a0e36-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="a0e36-133">AQS no EWS dá suporte a três tipos de restrições: restrição de fase de palavra, restrição de intervalo de datas e restrição de tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="a0e36-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="a0e36-134">As tabelas a seguir listam as propriedades de pesquisa suportadas para cada tipo de restrição.</span><span class="sxs-lookup"><span data-stu-id="a0e36-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="a0e36-135">**Restrição de fase do Word**</span><span class="sxs-lookup"><span data-stu-id="a0e36-135">**Word phase restriction**</span></span>

|<span data-ttu-id="a0e36-136">**Propriedade**</span><span class="sxs-lookup"><span data-stu-id="a0e36-136">**Property**</span></span>|<span data-ttu-id="a0e36-137">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="a0e36-137">**Example**</span></span>|<span data-ttu-id="a0e36-138">**Function**</span><span class="sxs-lookup"><span data-stu-id="a0e36-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0e36-139">from</span><span class="sxs-lookup"><span data-stu-id="a0e36-139">from</span></span>  <br/> |<span data-ttu-id="a0e36-140">De: diretora</span><span class="sxs-lookup"><span data-stu-id="a0e36-140">From:Dean</span></span>  <br/> <span data-ttu-id="a0e36-141">De: "Halstead"</span><span class="sxs-lookup"><span data-stu-id="a0e36-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="a0e36-142">Itens de pesquisa enviados pelo diretor.</span><span class="sxs-lookup"><span data-stu-id="a0e36-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="a0e36-143">Itens de pesquisa enviados por Halstead.</span><span class="sxs-lookup"><span data-stu-id="a0e36-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="a0e36-144">O remetente deve ser exatamente "Halstead".</span><span class="sxs-lookup"><span data-stu-id="a0e36-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="a0e36-145">para</span><span class="sxs-lookup"><span data-stu-id="a0e36-145">to</span></span>  <br/> |<span data-ttu-id="a0e36-146">Para: diretora</span><span class="sxs-lookup"><span data-stu-id="a0e36-146">To:Dean</span></span>  <br/> |<span data-ttu-id="a0e36-147">Itens de pesquisa enviados para a diretora.</span><span class="sxs-lookup"><span data-stu-id="a0e36-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="a0e36-148">cc</span><span class="sxs-lookup"><span data-stu-id="a0e36-148">cc</span></span>  <br/> |<span data-ttu-id="a0e36-149">CC: diretora</span><span class="sxs-lookup"><span data-stu-id="a0e36-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="a0e36-150">Pesquise itens com o diretor na linha CC.</span><span class="sxs-lookup"><span data-stu-id="a0e36-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="a0e36-151">bcc</span><span class="sxs-lookup"><span data-stu-id="a0e36-151">bcc</span></span>  <br/> |<span data-ttu-id="a0e36-152">CCO: diretora</span><span class="sxs-lookup"><span data-stu-id="a0e36-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="a0e36-153">Pesquisar itens com a linha de um na linha Cco.</span><span class="sxs-lookup"><span data-stu-id="a0e36-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="a0e36-154">Participante</span><span class="sxs-lookup"><span data-stu-id="a0e36-154">Participants</span></span>  <br/> |<span data-ttu-id="a0e36-155">Participantes: diretora</span><span class="sxs-lookup"><span data-stu-id="a0e36-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="a0e36-156">Pesquisar itens com o diretor nos campos para, CC ou Cco.</span><span class="sxs-lookup"><span data-stu-id="a0e36-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="a0e36-157">Assunto</span><span class="sxs-lookup"><span data-stu-id="a0e36-157">Subject</span></span>  <br/> |<span data-ttu-id="a0e36-158">Assunto: produto</span><span class="sxs-lookup"><span data-stu-id="a0e36-158">Subject:product</span></span>  <br/> <span data-ttu-id="a0e36-159">Assunto: (desenvolvimento de produtos)</span><span class="sxs-lookup"><span data-stu-id="a0e36-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="a0e36-160">Assunto: "desenvolvimento de produtos"</span><span class="sxs-lookup"><span data-stu-id="a0e36-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="a0e36-161">Pesquisar itens com o produto no assunto.</span><span class="sxs-lookup"><span data-stu-id="a0e36-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="a0e36-162">Pesquisar itens com produtos e desenvolvimento no assunto.</span><span class="sxs-lookup"><span data-stu-id="a0e36-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="a0e36-163">Corpo</span><span class="sxs-lookup"><span data-stu-id="a0e36-163">Body</span></span>  <br/> <span data-ttu-id="a0e36-164">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="a0e36-164">Content</span></span>  <br/> |<span data-ttu-id="a0e36-165">Corpo: Progress</span><span class="sxs-lookup"><span data-stu-id="a0e36-165">Body:progress</span></span>  <br/> <span data-ttu-id="a0e36-166">Conteúdo: progresso</span><span class="sxs-lookup"><span data-stu-id="a0e36-166">Content:progress</span></span>  <br/> |<span data-ttu-id="a0e36-167">Pesquisar itens com progresso no corpo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="a0e36-168">Anexo</span><span class="sxs-lookup"><span data-stu-id="a0e36-168">Attachment</span></span>  <br/> |<span data-ttu-id="a0e36-169">Anexo: relatório</span><span class="sxs-lookup"><span data-stu-id="a0e36-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="a0e36-170">Pesquisar itens com o relatório no nome do arquivo de anexo ou no corpo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="a0e36-171">(Propriedade não especificada)</span><span class="sxs-lookup"><span data-stu-id="a0e36-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="a0e36-172">Desenvolvimento de produtos</span><span class="sxs-lookup"><span data-stu-id="a0e36-172">Product Development</span></span>  <br/> |<span data-ttu-id="a0e36-173">Pesquisar itens que contenham produtos e desenvolvimento em todas as propriedades da fase do Word.</span><span class="sxs-lookup"><span data-stu-id="a0e36-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="a0e36-174">A correspondência de restrição de fase de palavra sempre diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="a0e36-175">A restrição de fase do Word dá suporte a dois tipos de correspondência: correspondência de prefixo ou correspondência exata.</span><span class="sxs-lookup"><span data-stu-id="a0e36-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="a0e36-176">O prefixo correspondente é o comportamento padrão de correspondência.</span><span class="sxs-lookup"><span data-stu-id="a0e36-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="a0e36-177">Se quiser correspondência exata, use aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="a0e36-178">Por exemplo, Subject: "Product" corresponde a "Product", mas não a "Production" no assunto.</span><span class="sxs-lookup"><span data-stu-id="a0e36-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="a0e36-179">Várias palavras em aspas duplas restringem ambas as fases da palavra e sua ordem.</span><span class="sxs-lookup"><span data-stu-id="a0e36-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="a0e36-180">Por exemplo, "produto de vitória" corresponde somente a "produto Win", não ' produto do Win95 ' ou "produto de vitória".</span><span class="sxs-lookup"><span data-stu-id="a0e36-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="a0e36-181">Você pode usar um asterisco ( \* ) para definir uma correspondência de prefixo com ordem restrita.</span><span class="sxs-lookup"><span data-stu-id="a0e36-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="a0e36-182">Por exemplo, "produto do Win" corresponde a " \* produto do Win95", "linha de produção do Windows", mas não "novo produto do Windows" ou "produto de vitória".</span><span class="sxs-lookup"><span data-stu-id="a0e36-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="a0e36-183">Você pode pesquisar todas as mensagens enviadas de ou para um domínio.</span><span class="sxs-lookup"><span data-stu-id="a0e36-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="a0e36-184">Por exemplo, de: "@hotmail. com" retorna todas as mensagens enviadas de hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="a0e36-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="a0e36-185">A tabela a seguir descreve as restrições de intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="a0e36-186">**Restrição de intervalo de datas**</span><span class="sxs-lookup"><span data-stu-id="a0e36-186">**Date range restriction**</span></span>

|<span data-ttu-id="a0e36-187">**Propriedade**</span><span class="sxs-lookup"><span data-stu-id="a0e36-187">**Property**</span></span>|<span data-ttu-id="a0e36-188">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="a0e36-188">**Example**</span></span>|<span data-ttu-id="a0e36-189">**Function**</span><span class="sxs-lookup"><span data-stu-id="a0e36-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0e36-190">Sent</span><span class="sxs-lookup"><span data-stu-id="a0e36-190">Sent</span></span>  <br/> |<span data-ttu-id="a0e36-191">Enviado: última semana</span><span class="sxs-lookup"><span data-stu-id="a0e36-191">Sent:last week</span></span>  <br/> <span data-ttu-id="a0e36-192">Enviado: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="a0e36-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="a0e36-193">Enviado: 01/01/2001.. 01/15/2001</span><span class="sxs-lookup"><span data-stu-id="a0e36-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="a0e36-194">Itens de pesquisa enviados na semana passada.</span><span class="sxs-lookup"><span data-stu-id="a0e36-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="a0e36-195">Itens de pesquisa enviados no dia 1º de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="a0e36-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="a0e36-196">Itens de pesquisa enviados entre 1º de janeiro de 2001 e 15 de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="a0e36-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="a0e36-197">Received</span><span class="sxs-lookup"><span data-stu-id="a0e36-197">Received</span></span>  <br/> |<span data-ttu-id="a0e36-198">Recebido: hoje</span><span class="sxs-lookup"><span data-stu-id="a0e36-198">Received:today</span></span>  <br/> <span data-ttu-id="a0e36-199">Recebido: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="a0e36-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="a0e36-200">Itens de pesquisa recebidos hoje.</span><span class="sxs-lookup"><span data-stu-id="a0e36-200">Search items received today.</span></span>  <br/> <span data-ttu-id="a0e36-201">Itens de pesquisa recebidos no dia 1º de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="a0e36-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="a0e36-202">Os dois pontos (..) são um operador de intervalo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="a0e36-203">Pode ser usado para definir um intervalo com um início e uma data de término.</span><span class="sxs-lookup"><span data-stu-id="a0e36-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="a0e36-204">Para especificar uma data, você pode usar datas relativas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="a0e36-205">As seguintes datas relativas têm suporte:</span><span class="sxs-lookup"><span data-stu-id="a0e36-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="a0e36-206">Datas relativas: hoje, amanhã, ontem</span><span class="sxs-lookup"><span data-stu-id="a0e36-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="a0e36-207">Datas relativas de MultiWord: esta semana, mês seguinte, semana passada, mês ou ano que vem</span><span class="sxs-lookup"><span data-stu-id="a0e36-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="a0e36-208">Dias: domingo, segunda-feira, terça-feira, quarta-feira, quinta-feira, sábado</span><span class="sxs-lookup"><span data-stu-id="a0e36-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="a0e36-209">Janeiro, fevereiro, março, abril, maio, junho de julho, agosto, setembro, outubro, novembro de dezembro</span><span class="sxs-lookup"><span data-stu-id="a0e36-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="a0e36-210">A tabela a seguir descreve as restrições de tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="a0e36-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="a0e36-211">**Restrição de tipo de mensagem**</span><span class="sxs-lookup"><span data-stu-id="a0e36-211">**Message type restriction**</span></span>

|<span data-ttu-id="a0e36-212">**Propriedade**</span><span class="sxs-lookup"><span data-stu-id="a0e36-212">**Property**</span></span>|<span data-ttu-id="a0e36-213">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="a0e36-213">**Example**</span></span>|<span data-ttu-id="a0e36-214">**Function**</span><span class="sxs-lookup"><span data-stu-id="a0e36-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0e36-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e36-215">Kind</span></span>  <br/> |<span data-ttu-id="a0e36-216">Tipo: tarefas</span><span class="sxs-lookup"><span data-stu-id="a0e36-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="a0e36-217">Pesquisar todos os itens de tarefa.</span><span class="sxs-lookup"><span data-stu-id="a0e36-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="a0e36-218">AQS no EWS usa a propriedade **Kind** para especificar o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="a0e36-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="a0e36-219">A propriedade Kind pode ser usada com os seguintes tipos de item:</span><span class="sxs-lookup"><span data-stu-id="a0e36-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="a0e36-220">email</span><span class="sxs-lookup"><span data-stu-id="a0e36-220">email</span></span>
    
- <span data-ttu-id="a0e36-221">treinamento</span><span class="sxs-lookup"><span data-stu-id="a0e36-221">meetings</span></span>
    
- <span data-ttu-id="a0e36-222">tarefas</span><span class="sxs-lookup"><span data-stu-id="a0e36-222">tasks</span></span>
    
- <span data-ttu-id="a0e36-223">notes</span><span class="sxs-lookup"><span data-stu-id="a0e36-223">notes</span></span>
    
- <span data-ttu-id="a0e36-224">docs</span><span class="sxs-lookup"><span data-stu-id="a0e36-224">docs</span></span>
    
- <span data-ttu-id="a0e36-225">diários</span><span class="sxs-lookup"><span data-stu-id="a0e36-225">journals</span></span>
    
- <span data-ttu-id="a0e36-226">contacts</span><span class="sxs-lookup"><span data-stu-id="a0e36-226">contacts</span></span>
    
- <span data-ttu-id="a0e36-227">respectiva</span><span class="sxs-lookup"><span data-stu-id="a0e36-227">im</span></span>
    
<span data-ttu-id="a0e36-228">A tabela a seguir descreve o agrupamento de conectores lógicos.</span><span class="sxs-lookup"><span data-stu-id="a0e36-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="a0e36-229">**Agrupando conectores lógicos**</span><span class="sxs-lookup"><span data-stu-id="a0e36-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="a0e36-230">**Connector**</span><span class="sxs-lookup"><span data-stu-id="a0e36-230">**Connector**</span></span>|<span data-ttu-id="a0e36-231">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="a0e36-231">**Example**</span></span>|<span data-ttu-id="a0e36-232">**Function**</span><span class="sxs-lookup"><span data-stu-id="a0e36-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0e36-233">E</span><span class="sxs-lookup"><span data-stu-id="a0e36-233">AND</span></span>  <br/> |<span data-ttu-id="a0e36-234">Assunto: produto e assunto: desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="a0e36-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="a0e36-235">Assunto: (produto e desenvolvimento)</span><span class="sxs-lookup"><span data-stu-id="a0e36-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="a0e36-236">Assunto: (desenvolvimento de produtos)</span><span class="sxs-lookup"><span data-stu-id="a0e36-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="a0e36-237">Pesquisar itens com produtos e desenvolvimento no assunto.</span><span class="sxs-lookup"><span data-stu-id="a0e36-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="a0e36-238">OU</span><span class="sxs-lookup"><span data-stu-id="a0e36-238">OR</span></span>  <br/> |<span data-ttu-id="a0e36-239">Corpo: projeto ou corpo: proposta</span><span class="sxs-lookup"><span data-stu-id="a0e36-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="a0e36-240">Corpo: (projeto ou proposta)</span><span class="sxs-lookup"><span data-stu-id="a0e36-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="a0e36-241">Pesquisar itens com o produto ou o desenvolvimento no corpo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="a0e36-242">NÃO</span><span class="sxs-lookup"><span data-stu-id="a0e36-242">NOT</span></span>  <br/> |<span data-ttu-id="a0e36-243">Não corpo: proposta</span><span class="sxs-lookup"><span data-stu-id="a0e36-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="a0e36-244">Corpo: (não proposta)</span><span class="sxs-lookup"><span data-stu-id="a0e36-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="a0e36-245">Pesquisar mensagens sem proposta no corpo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="a0e36-246">E é sempre o conector padrão.</span><span class="sxs-lookup"><span data-stu-id="a0e36-246">AND is always the default connector.</span></span> <span data-ttu-id="a0e36-247">Por exemplo, Subject: Project e Body: proposta é o mesmo que o assunto: corpo do projeto: proposta.</span><span class="sxs-lookup"><span data-stu-id="a0e36-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="a0e36-248">Conectores lógicos diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="a0e36-249">Por exemplo, corpo: (projeto ou proposta) pesquisa mensagens com "projeto", "ou" e "proposta" no corpo em vez de "projeto" ou "proposta".</span><span class="sxs-lookup"><span data-stu-id="a0e36-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="a0e36-250">O símbolo de adição (+) equivale a e.</span><span class="sxs-lookup"><span data-stu-id="a0e36-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="a0e36-251">O símbolo de hífen (-) é equivalente a não.</span><span class="sxs-lookup"><span data-stu-id="a0e36-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="a0e36-252">Por exemplo, Body: (Project-propostas) pesquisa mensagens com "Project", mas sem "proposta" no corpo.</span><span class="sxs-lookup"><span data-stu-id="a0e36-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="a0e36-253">A cadeia de caracteres de consulta também pode conter Propriedades não indexadas para pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a0e36-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="a0e36-254">Se a cadeia de caracteres de consulta contiver Propriedades não indexadas, a pesquisa poderá realizar uma pesquisa do Exchange nas propriedades indexadas e uma pesquisa de armazenamento nas propriedades não indexadas.</span><span class="sxs-lookup"><span data-stu-id="a0e36-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="a0e36-255">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0e36-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="a0e36-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0e36-256">Example</span></span>

<span data-ttu-id="a0e36-257">O exemplo a seguir mostra uma solicitação de pesquisa de mensagens na caixa de entrada com descoberta automática no assunto.</span><span class="sxs-lookup"><span data-stu-id="a0e36-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a0e36-258">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0e36-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a><span data-ttu-id="a0e36-259">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a0e36-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0e36-260">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0e36-260">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0e36-261">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0e36-261">Schema name</span></span>  <br/> |<span data-ttu-id="a0e36-262">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a0e36-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0e36-263">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0e36-263">Validation file</span></span>  <br/> |<span data-ttu-id="a0e36-264">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0e36-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0e36-265">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a0e36-265">Can be empty</span></span>  <br/> |<span data-ttu-id="a0e36-266">False</span><span class="sxs-lookup"><span data-stu-id="a0e36-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0e36-267">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0e36-267">See also</span></span>



[<span data-ttu-id="a0e36-268">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="a0e36-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="a0e36-269">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="a0e36-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="a0e36-270">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a0e36-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

