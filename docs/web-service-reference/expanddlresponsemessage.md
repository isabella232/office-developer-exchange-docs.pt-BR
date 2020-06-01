---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: O elemento ExpandDLResponseMessage contém o status e o resultado de uma única solicitação de operação de ExpandDL.
ms.openlocfilehash: e186c4e14cbb9c922a4d262c85c130b9c33ff939
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460635"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="18aab-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="18aab-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="18aab-104">O elemento **ExpandDLResponseMessage** contém o status e o resultado de uma única solicitação de [operação de ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="18aab-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="18aab-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="18aab-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="18aab-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="18aab-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="18aab-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="18aab-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="18aab-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="18aab-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="18aab-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="18aab-109">Attributes and elements</span></span>

<span data-ttu-id="18aab-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="18aab-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18aab-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="18aab-111">Attributes</span></span>

|<span data-ttu-id="18aab-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="18aab-112">**Attribute**</span></span>|<span data-ttu-id="18aab-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18aab-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18aab-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="18aab-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="18aab-115">Descreve o status de uma resposta de [operação do ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="18aab-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="18aab-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="18aab-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="18aab-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="18aab-117">-  Success</span></span>  <br/><span data-ttu-id="18aab-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="18aab-118">-  Warning</span></span>  <br/><span data-ttu-id="18aab-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="18aab-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="18aab-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="18aab-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="18aab-121">Representa o próximo índice que deve ser usado para a próxima solicitação quando um modo de exibição de paginação indexado é usado.</span><span class="sxs-lookup"><span data-stu-id="18aab-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="18aab-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="18aab-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="18aab-123">Representa o novo valor do numerador a ser usado para a próxima solicitação quando os modos de exibição de página de fração são usados.</span><span class="sxs-lookup"><span data-stu-id="18aab-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="18aab-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="18aab-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="18aab-125">Representa o próximo denominador a ser usado para a próxima solicitação ao fazer paginação fracionária.</span><span class="sxs-lookup"><span data-stu-id="18aab-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="18aab-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="18aab-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="18aab-127">Indica que a paginação adicional não é necessária.</span><span class="sxs-lookup"><span data-stu-id="18aab-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="18aab-128">Este atributo será true se os resultados atuais contiverem o último item na consulta.</span><span class="sxs-lookup"><span data-stu-id="18aab-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="18aab-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="18aab-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="18aab-130">Representa o número total de itens que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="18aab-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="18aab-131">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="18aab-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="18aab-132">**Valor**</span><span class="sxs-lookup"><span data-stu-id="18aab-132">**Value**</span></span>|<span data-ttu-id="18aab-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18aab-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18aab-134">**Success**</span><span class="sxs-lookup"><span data-stu-id="18aab-134">**Success**</span></span> <br/> |<span data-ttu-id="18aab-135">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="18aab-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="18aab-136">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="18aab-136">**Warning**</span></span> <br/> | <span data-ttu-id="18aab-137">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="18aab-137">Describes a request that was not processed.</span></span> <span data-ttu-id="18aab-138">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="18aab-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="18aab-139">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="18aab-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="18aab-140">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="18aab-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="18aab-141">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="18aab-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="18aab-142">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="18aab-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="18aab-143">– O banco de dados de caixa de correio (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="18aab-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="18aab-144">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="18aab-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="18aab-145">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="18aab-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="18aab-146">**Error**</span><span class="sxs-lookup"><span data-stu-id="18aab-146">**Error**</span></span> <br/> | <span data-ttu-id="18aab-147">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="18aab-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="18aab-148">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="18aab-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="18aab-149">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="18aab-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="18aab-150">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="18aab-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="18aab-151">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="18aab-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="18aab-152">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="18aab-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="18aab-153">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="18aab-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="18aab-154">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="18aab-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="18aab-155">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="18aab-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="18aab-156">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="18aab-156">Child elements</span></span>

|<span data-ttu-id="18aab-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18aab-157">**Element**</span></span>|<span data-ttu-id="18aab-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18aab-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18aab-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="18aab-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="18aab-160">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aab-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="18aab-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="18aab-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="18aab-162">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="18aab-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="18aab-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="18aab-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="18aab-164">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="18aab-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="18aab-165">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="18aab-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="18aab-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="18aab-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="18aab-167">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="18aab-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="18aab-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="18aab-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="18aab-169">Contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="18aab-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18aab-170">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="18aab-170">Parent elements</span></span>

|<span data-ttu-id="18aab-171">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18aab-171">**Element**</span></span>|<span data-ttu-id="18aab-172">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18aab-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18aab-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="18aab-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="18aab-174">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18aab-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18aab-175">Comentários</span><span class="sxs-lookup"><span data-stu-id="18aab-175">Remarks</span></span>

<span data-ttu-id="18aab-176">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="18aab-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18aab-177">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="18aab-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18aab-178">Namespace</span><span class="sxs-lookup"><span data-stu-id="18aab-178">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18aab-179">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="18aab-179">Schema Name</span></span>  <br/> |<span data-ttu-id="18aab-180">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="18aab-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="18aab-181">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="18aab-181">Validation File</span></span>  <br/> |<span data-ttu-id="18aab-182">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="18aab-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18aab-183">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="18aab-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="18aab-184">False</span><span class="sxs-lookup"><span data-stu-id="18aab-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18aab-185">Confira também</span><span class="sxs-lookup"><span data-stu-id="18aab-185">See also</span></span>

- [<span data-ttu-id="18aab-186">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="18aab-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="18aab-187">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="18aab-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="18aab-188">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="18aab-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

