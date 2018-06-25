---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: O elemento de QueryString contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824943"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="ac167-103">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="ac167-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="ac167-104">O elemento de **QueryString** contém uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).</span><span class="sxs-lookup"><span data-stu-id="ac167-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="ac167-105">**QueryStringType**</span><span class="sxs-lookup"><span data-stu-id="ac167-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac167-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ac167-106">Attributes and elements</span></span>

<span data-ttu-id="ac167-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac167-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac167-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac167-108">Attributes</span></span>

|<span data-ttu-id="ac167-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="ac167-109">**Attribute**</span></span>|<span data-ttu-id="ac167-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac167-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ac167-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="ac167-111">ResetCache</span></span>  <br/> |<span data-ttu-id="ac167-112">Indica que o cache deve ser redefinido.</span><span class="sxs-lookup"><span data-stu-id="ac167-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="ac167-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="ac167-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="ac167-114">Indica que os itens excluídos devem ser retornados.</span><span class="sxs-lookup"><span data-stu-id="ac167-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="ac167-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="ac167-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="ac167-116">Indica que os termos realçados devem ser retornados.</span><span class="sxs-lookup"><span data-stu-id="ac167-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ac167-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac167-117">Child elements</span></span>

<span data-ttu-id="ac167-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac167-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac167-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac167-119">Parent elements</span></span>

|<span data-ttu-id="ac167-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac167-120">**Element**</span></span>|<span data-ttu-id="ac167-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac167-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac167-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="ac167-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ac167-123">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ac167-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="ac167-124">A seguir é a expressão XPath para esse elemento: /FindItem.</span><span class="sxs-lookup"><span data-stu-id="ac167-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac167-125">Text value</span><span class="sxs-lookup"><span data-stu-id="ac167-125">Text value</span></span>

<span data-ttu-id="ac167-126">O valor de texto do elemento **QueryString** representa uma consulta de caixa de correio que será feita usando um subconjunto da [Sintaxe de consulta avançada (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ac167-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="ac167-127">Consulte a seção de comentários para obter informações sobre as opções de sintaxe com suporte para cadeias de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="ac167-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac167-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac167-128">Remarks</span></span>

<span data-ttu-id="ac167-129">No Exchange Server 2010, esse elemento é um tipo de cadeia de caracteres de esquema XML.</span><span class="sxs-lookup"><span data-stu-id="ac167-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="ac167-130">Nas versões do Exchange, começando com o Exchange Server 2013, incluindo o Exchange Online, o tipo deste elemento é **QueryStringType**.</span><span class="sxs-lookup"><span data-stu-id="ac167-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="ac167-131">Essa alteração não quebrará quaisquer clientes existentes, pois adiciona três novos atributos opcionais.</span><span class="sxs-lookup"><span data-stu-id="ac167-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="ac167-132">O elemento **QueryString** exclui o uso das restrições do EWS.</span><span class="sxs-lookup"><span data-stu-id="ac167-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="ac167-133">AQS no EWS oferece suporte a três tipos de restrições: restrição de fase, a restrição de intervalo de data e a restrição de tipo de mensagem do word.</span><span class="sxs-lookup"><span data-stu-id="ac167-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="ac167-134">As tabelas a seguir listam as propriedades de pesquisa com suporte para cada tipo de restrição.</span><span class="sxs-lookup"><span data-stu-id="ac167-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="ac167-135">**Restrição de fase do Word**</span><span class="sxs-lookup"><span data-stu-id="ac167-135">**Word phase restriction**</span></span>

|<span data-ttu-id="ac167-136">**Property**</span><span class="sxs-lookup"><span data-stu-id="ac167-136">**Property**</span></span>|<span data-ttu-id="ac167-137">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="ac167-137">**Example**</span></span>|<span data-ttu-id="ac167-138">**Function**</span><span class="sxs-lookup"><span data-stu-id="ac167-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ac167-139">from</span><span class="sxs-lookup"><span data-stu-id="ac167-139">from</span></span>  <br/> |<span data-ttu-id="ac167-140">De: Dean</span><span class="sxs-lookup"><span data-stu-id="ac167-140">From:Dean</span></span>  <br/> <span data-ttu-id="ac167-141">De: "Dean Halstead"</span><span class="sxs-lookup"><span data-stu-id="ac167-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="ac167-142">Pesquisar os itens enviados do Dean.</span><span class="sxs-lookup"><span data-stu-id="ac167-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="ac167-143">Pesquisar os itens enviados do Dean Halstead.</span><span class="sxs-lookup"><span data-stu-id="ac167-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="ac167-144">O remetente deve ser exatamente "Dean Halstead".</span><span class="sxs-lookup"><span data-stu-id="ac167-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="ac167-145">para</span><span class="sxs-lookup"><span data-stu-id="ac167-145">to</span></span>  <br/> |<span data-ttu-id="ac167-146">Como: Dean</span><span class="sxs-lookup"><span data-stu-id="ac167-146">To:Dean</span></span>  <br/> |<span data-ttu-id="ac167-147">Pesquisar os itens enviados para Dean.</span><span class="sxs-lookup"><span data-stu-id="ac167-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="ac167-148">cc</span><span class="sxs-lookup"><span data-stu-id="ac167-148">cc</span></span>  <br/> |<span data-ttu-id="ac167-149">Cc:Dean</span><span class="sxs-lookup"><span data-stu-id="ac167-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="ac167-150">Procurar itens com Dean na linha Cc.</span><span class="sxs-lookup"><span data-stu-id="ac167-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="ac167-151">bcc</span><span class="sxs-lookup"><span data-stu-id="ac167-151">bcc</span></span>  <br/> |<span data-ttu-id="ac167-152">BCC:Dean</span><span class="sxs-lookup"><span data-stu-id="ac167-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="ac167-153">Procurar itens com Dean na linha Cco.</span><span class="sxs-lookup"><span data-stu-id="ac167-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="ac167-154">Participantes</span><span class="sxs-lookup"><span data-stu-id="ac167-154">Participants</span></span>  <br/> |<span data-ttu-id="ac167-155">Participantes: Dean</span><span class="sxs-lookup"><span data-stu-id="ac167-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="ac167-156">Pesquisar itens com Dean para, Cc ou Cco, campos.</span><span class="sxs-lookup"><span data-stu-id="ac167-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="ac167-157">Assunto</span><span class="sxs-lookup"><span data-stu-id="ac167-157">Subject</span></span>  <br/> |<span data-ttu-id="ac167-158">Assunto: produto</span><span class="sxs-lookup"><span data-stu-id="ac167-158">Subject:product</span></span>  <br/> <span data-ttu-id="ac167-159">Assunto:(product development)</span><span class="sxs-lookup"><span data-stu-id="ac167-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="ac167-160">Assunto: "desenvolvimento do produto"</span><span class="sxs-lookup"><span data-stu-id="ac167-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="ac167-161">Procurar itens com o produto no assunto.</span><span class="sxs-lookup"><span data-stu-id="ac167-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="ac167-162">Procurar itens com o produto e desenvolvimento no assunto.</span><span class="sxs-lookup"><span data-stu-id="ac167-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="ac167-163">Body</span><span class="sxs-lookup"><span data-stu-id="ac167-163">Body</span></span>  <br/> <span data-ttu-id="ac167-164">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="ac167-164">Content</span></span>  <br/> |<span data-ttu-id="ac167-165">Corpo: progresso</span><span class="sxs-lookup"><span data-stu-id="ac167-165">Body:progress</span></span>  <br/> <span data-ttu-id="ac167-166">Progresso de conteúdo:</span><span class="sxs-lookup"><span data-stu-id="ac167-166">Content:progress</span></span>  <br/> |<span data-ttu-id="ac167-167">Procurar itens cujo andamento no corpo.</span><span class="sxs-lookup"><span data-stu-id="ac167-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="ac167-168">Anexo</span><span class="sxs-lookup"><span data-stu-id="ac167-168">Attachment</span></span>  <br/> |<span data-ttu-id="ac167-169">Anexo: relatório</span><span class="sxs-lookup"><span data-stu-id="ac167-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="ac167-170">Procurar itens com o relatório no corpo de arquivo ou nome de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac167-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="ac167-171">(a propriedade não for especificada)</span><span class="sxs-lookup"><span data-stu-id="ac167-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="ac167-172">Desenvolvimento do produto</span><span class="sxs-lookup"><span data-stu-id="ac167-172">Product Development</span></span>  <br/> |<span data-ttu-id="ac167-173">Procurar itens que contenham o produto e desenvolvimento em todas as propriedades de fase do word.</span><span class="sxs-lookup"><span data-stu-id="ac167-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="ac167-174">Correspondência de restrição do Word fase sempre diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ac167-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="ac167-175">Restrição de fase do Word suporta dois tipos de correspondência: correspondência de prefixo ou correspondência exata.</span><span class="sxs-lookup"><span data-stu-id="ac167-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="ac167-176">Correspondência de prefixo é o comportamento padrão de correspondência.</span><span class="sxs-lookup"><span data-stu-id="ac167-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="ac167-177">Se você quiser correspondência exata, use aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="ac167-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="ac167-178">Por exemplo, subject: corresponde a "product" 'produto', mas não 'produção' no assunto.</span><span class="sxs-lookup"><span data-stu-id="ac167-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="ac167-179">Várias palavras em aspas duplas restringem fases do word e sua ordem.</span><span class="sxs-lookup"><span data-stu-id="ac167-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="ac167-180">Por exemplo "win produto" corresponde a única 'win produto', não 'win95 produto' ou 'produto do win'.</span><span class="sxs-lookup"><span data-stu-id="ac167-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="ac167-181">Você pode usar um asterisco (\*) para definir uma correspondência de prefixo com ordem restringido.</span><span class="sxs-lookup"><span data-stu-id="ac167-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="ac167-182">Por exemplo, "win produto"\* corresponde 'win95 produto', 'linha de produção do windows', mas não 'windows novo produto' ou 'produto do win'.</span><span class="sxs-lookup"><span data-stu-id="ac167-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="ac167-183">Você pode pesquisar todas as mensagens enviadas de ou para um domínio.</span><span class="sxs-lookup"><span data-stu-id="ac167-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="ac167-184">Por exemplo, from:"@hotmail.com" retorna todas as mensagens enviadas de hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="ac167-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="ac167-185">A tabela a seguir descreve as restrições de intervalo de data.</span><span class="sxs-lookup"><span data-stu-id="ac167-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="ac167-186">**Restrição de intervalo de data**</span><span class="sxs-lookup"><span data-stu-id="ac167-186">**Date range restriction**</span></span>

|<span data-ttu-id="ac167-187">**Property**</span><span class="sxs-lookup"><span data-stu-id="ac167-187">**Property**</span></span>|<span data-ttu-id="ac167-188">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="ac167-188">**Example**</span></span>|<span data-ttu-id="ac167-189">**Function**</span><span class="sxs-lookup"><span data-stu-id="ac167-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ac167-190">Enviado</span><span class="sxs-lookup"><span data-stu-id="ac167-190">Sent</span></span>  <br/> |<span data-ttu-id="ac167-191">Enviados: última semana</span><span class="sxs-lookup"><span data-stu-id="ac167-191">Sent:last week</span></span>  <br/> <span data-ttu-id="ac167-192">Enviados: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="ac167-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="ac167-193">Sent:01/01/2001..01/15/2001</span><span class="sxs-lookup"><span data-stu-id="ac167-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="ac167-194">Pesquisar itens enviados a última semana.</span><span class="sxs-lookup"><span data-stu-id="ac167-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="ac167-195">Pesquisar os itens enviados em 1º de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="ac167-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="ac167-196">Pesquisar os itens enviados entre 1º de janeiro de 2001 e 15 de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="ac167-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="ac167-197">Received</span><span class="sxs-lookup"><span data-stu-id="ac167-197">Received</span></span>  <br/> |<span data-ttu-id="ac167-198">Recebidos: hoje</span><span class="sxs-lookup"><span data-stu-id="ac167-198">Received:today</span></span>  <br/> <span data-ttu-id="ac167-199">Recebidos: 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="ac167-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="ac167-200">Pesquisar os itens recebidas hoje.</span><span class="sxs-lookup"><span data-stu-id="ac167-200">Search items received today.</span></span>  <br/> <span data-ttu-id="ac167-201">Pesquisar itens recebidos em 1º de janeiro de 2001.</span><span class="sxs-lookup"><span data-stu-id="ac167-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="ac167-202">Os dois pontos (.) é um operador de intervalo.</span><span class="sxs-lookup"><span data-stu-id="ac167-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="ac167-203">Ele pode ser usado para definir um intervalo com um início e uma data de término.</span><span class="sxs-lookup"><span data-stu-id="ac167-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="ac167-204">Para especificar uma data, você pode usar datas relativas.</span><span class="sxs-lookup"><span data-stu-id="ac167-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="ac167-205">Há suporte para as seguintes datas relativas:</span><span class="sxs-lookup"><span data-stu-id="ac167-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="ac167-206">Datas relativas: hoje, amanhã, ontem</span><span class="sxs-lookup"><span data-stu-id="ac167-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="ac167-207">Datas relativas multiword: esta semana, mês seguinte, última semana, passou do mês ou ano seguinte</span><span class="sxs-lookup"><span data-stu-id="ac167-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="ac167-208">Dias: Domingo, segunda-feira, terça-feira, quarta-feira, quinta-feira, sexta-feira, sábado</span><span class="sxs-lookup"><span data-stu-id="ac167-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="ac167-209">Janeiro, fevereiro e março, abril, maio, junho, julho, agosto, setembro, outubro, novembro, dezembro</span><span class="sxs-lookup"><span data-stu-id="ac167-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="ac167-210">A tabela a seguir descreve as restrições de tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="ac167-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="ac167-211">**Restrição de tipo de mensagem**</span><span class="sxs-lookup"><span data-stu-id="ac167-211">**Message type restriction**</span></span>

|<span data-ttu-id="ac167-212">**Property**</span><span class="sxs-lookup"><span data-stu-id="ac167-212">**Property**</span></span>|<span data-ttu-id="ac167-213">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="ac167-213">**Example**</span></span>|<span data-ttu-id="ac167-214">**Function**</span><span class="sxs-lookup"><span data-stu-id="ac167-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ac167-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac167-215">Kind</span></span>  <br/> |<span data-ttu-id="ac167-216">Tipo: tarefas</span><span class="sxs-lookup"><span data-stu-id="ac167-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="ac167-217">Pesquise todos os itens de tarefa.</span><span class="sxs-lookup"><span data-stu-id="ac167-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="ac167-218">AQS no EWS usa a propriedade **Kind** para especificar o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="ac167-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="ac167-219">A propriedade Kind pode ser usada com os seguintes tipos de item:</span><span class="sxs-lookup"><span data-stu-id="ac167-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="ac167-220">email</span><span class="sxs-lookup"><span data-stu-id="ac167-220">email</span></span>
    
- <span data-ttu-id="ac167-221">reuniões</span><span class="sxs-lookup"><span data-stu-id="ac167-221">meetings</span></span>
    
- <span data-ttu-id="ac167-222">tarefas</span><span class="sxs-lookup"><span data-stu-id="ac167-222">tasks</span></span>
    
- <span data-ttu-id="ac167-223">Observações</span><span class="sxs-lookup"><span data-stu-id="ac167-223">notes</span></span>
    
- <span data-ttu-id="ac167-224">documentos</span><span class="sxs-lookup"><span data-stu-id="ac167-224">docs</span></span>
    
- <span data-ttu-id="ac167-225">diários</span><span class="sxs-lookup"><span data-stu-id="ac167-225">journals</span></span>
    
- <span data-ttu-id="ac167-226">contatos</span><span class="sxs-lookup"><span data-stu-id="ac167-226">contacts</span></span>
    
- <span data-ttu-id="ac167-227">mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="ac167-227">im</span></span>
    
<span data-ttu-id="ac167-228">A tabela a seguir descreve o agrupamento lógicos conectores.</span><span class="sxs-lookup"><span data-stu-id="ac167-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="ac167-229">**Conectores de lógica de agrupamento**</span><span class="sxs-lookup"><span data-stu-id="ac167-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="ac167-230">**Conector**</span><span class="sxs-lookup"><span data-stu-id="ac167-230">**Connector**</span></span>|<span data-ttu-id="ac167-231">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="ac167-231">**Example**</span></span>|<span data-ttu-id="ac167-232">**Function**</span><span class="sxs-lookup"><span data-stu-id="ac167-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ac167-233">E</span><span class="sxs-lookup"><span data-stu-id="ac167-233">AND</span></span>  <br/> |<span data-ttu-id="ac167-234">Assunto: produto e assunto: desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="ac167-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="ac167-235">Assunto:(product AND development)</span><span class="sxs-lookup"><span data-stu-id="ac167-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="ac167-236">Assunto:(product development)</span><span class="sxs-lookup"><span data-stu-id="ac167-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="ac167-237">Pesquisar os itens com o produto e desenvolvimento no assunto.</span><span class="sxs-lookup"><span data-stu-id="ac167-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="ac167-238">OU</span><span class="sxs-lookup"><span data-stu-id="ac167-238">OR</span></span>  <br/> |<span data-ttu-id="ac167-239">Corpo: projeto ou corpo: proposta</span><span class="sxs-lookup"><span data-stu-id="ac167-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="ac167-240">Corpo:(project OR proposal)</span><span class="sxs-lookup"><span data-stu-id="ac167-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="ac167-241">Pesquisar os itens com o produto ou desenvolvimento no corpo.</span><span class="sxs-lookup"><span data-stu-id="ac167-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="ac167-242">NÃO</span><span class="sxs-lookup"><span data-stu-id="ac167-242">NOT</span></span>  <br/> |<span data-ttu-id="ac167-243">NÃO corpo: proposta</span><span class="sxs-lookup"><span data-stu-id="ac167-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="ac167-244">Corpo:(NOT proposal)</span><span class="sxs-lookup"><span data-stu-id="ac167-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="ac167-245">Pesquisar mensagens sem proposta no corpo.</span><span class="sxs-lookup"><span data-stu-id="ac167-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="ac167-246">E é sempre o conector padrão.</span><span class="sxs-lookup"><span data-stu-id="ac167-246">AND is always the default connector.</span></span> <span data-ttu-id="ac167-247">Por exemplo, o assunto: projeto e corpo: proposta é o mesmo assunto: project corpo: proposta.</span><span class="sxs-lookup"><span data-stu-id="ac167-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="ac167-248">Conectores lógicas diferenciam maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ac167-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="ac167-249">Por exemplo, do corpo:(project Or proposal) procura mensagens com 'projeto', 'ou' e proposta no corpo, em vez de 'projeto' ou 'proposta'.</span><span class="sxs-lookup"><span data-stu-id="ac167-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="ac167-250">O símbolo de adição (+) é equivalente à and.</span><span class="sxs-lookup"><span data-stu-id="ac167-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="ac167-251">O símbolo de hífen (-) é equivalente à não.</span><span class="sxs-lookup"><span data-stu-id="ac167-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="ac167-252">Por exemplo, do corpo:(project-proposal) procura mensagens com 'projeto', mas sem 'proposta' no corpo.</span><span class="sxs-lookup"><span data-stu-id="ac167-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="ac167-253">A cadeia de caracteres de consulta também pode conter as propriedades não-indexadas para pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ac167-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="ac167-254">Se a cadeia de caracteres de consulta contém propriedades não-indexadas, a pesquisa pode executar uma pesquisa do Exchange sobre as propriedades indexadas e uma pesquisa de repositório de propriedades não-indexado.</span><span class="sxs-lookup"><span data-stu-id="ac167-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="ac167-255">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac167-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="ac167-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac167-256">Example</span></span>

<span data-ttu-id="ac167-257">O exemplo a seguir mostra uma solicitação para pesquisar mensagens na caixa de entrada com a descoberta automática no assunto.</span><span class="sxs-lookup"><span data-stu-id="ac167-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="ac167-258">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac167-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="ac167-259">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ac167-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac167-260">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac167-260">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac167-261">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ac167-261">Schema name</span></span>  <br/> |<span data-ttu-id="ac167-262">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ac167-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac167-263">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ac167-263">Validation file</span></span>  <br/> |<span data-ttu-id="ac167-264">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac167-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac167-265">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ac167-265">Can be empty</span></span>  <br/> |<span data-ttu-id="ac167-266">False</span><span class="sxs-lookup"><span data-stu-id="ac167-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac167-267">Ver também</span><span class="sxs-lookup"><span data-stu-id="ac167-267">See also</span></span>



[<span data-ttu-id="ac167-268">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="ac167-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="ac167-269">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="ac167-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="ac167-270">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ac167-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

