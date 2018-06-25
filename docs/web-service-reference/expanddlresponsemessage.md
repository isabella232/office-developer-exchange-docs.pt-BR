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
description: O elemento ExpandDLResponseMessage contém o status e o resultado de uma única solicitação de operação ExpandDL.
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752148"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="e966d-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e966d-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="e966d-104">O elemento **ExpandDLResponseMessage** contém o status e o resultado de uma única [operação ExpandDL](expanddl-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="e966d-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="e966d-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="e966d-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="e966d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e966d-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="e966d-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e966d-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="e966d-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e966d-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e966d-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e966d-109">Attributes and elements</span></span>

<span data-ttu-id="e966d-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e966d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e966d-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="e966d-111">Attributes</span></span>

|<span data-ttu-id="e966d-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e966d-112">**Attribute**</span></span>|<span data-ttu-id="e966d-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e966d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e966d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e966d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e966d-115">Descreve o status de uma resposta de [operação ExpandDL](expanddl-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e966d-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="e966d-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="e966d-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="e966d-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="e966d-117">-  Success</span></span>  <br/><span data-ttu-id="e966d-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="e966d-118">-  Warning</span></span>  <br/><span data-ttu-id="e966d-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="e966d-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="e966d-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="e966d-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="e966d-121">Representa o próximo índice que deve ser usado para a próxima solicitação quando o modo de exibição indexada paginação é usado.</span><span class="sxs-lookup"><span data-stu-id="e966d-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="e966d-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="e966d-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="e966d-123">Representa o novo valor numerador usada para a próxima solicitação quando fração exibições de página são usadas.</span><span class="sxs-lookup"><span data-stu-id="e966d-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="e966d-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="e966d-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="e966d-125">Representa o denominador próximo a ser usado para a próxima solicitação ao fazer a paginação fracional.</span><span class="sxs-lookup"><span data-stu-id="e966d-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="e966d-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="e966d-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="e966d-127">Indica que a paginação adicional não é necessária.</span><span class="sxs-lookup"><span data-stu-id="e966d-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="e966d-128">Este atributo será true se os resultados atuais contêm o último item na consulta.</span><span class="sxs-lookup"><span data-stu-id="e966d-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="e966d-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="e966d-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="e966d-130">Representa o número total de itens que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="e966d-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e966d-131">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e966d-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="e966d-132">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e966d-132">**Value**</span></span>|<span data-ttu-id="e966d-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e966d-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e966d-134">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="e966d-134">**Success**</span></span> <br/> |<span data-ttu-id="e966d-135">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="e966d-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e966d-136">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e966d-136">**Warning**</span></span> <br/> | <span data-ttu-id="e966d-137">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="e966d-137">Describes a request that was not processed.</span></span> <span data-ttu-id="e966d-138">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="e966d-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="e966d-139">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="e966d-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="e966d-140">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="e966d-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e966d-141">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="e966d-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e966d-142">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="e966d-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e966d-143">-O banco de dados de caixa de correio (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="e966d-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e966d-144">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="e966d-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="e966d-145">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="e966d-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="e966d-146">**Erro**</span><span class="sxs-lookup"><span data-stu-id="e966d-146">**Error**</span></span> <br/> | <span data-ttu-id="e966d-147">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="e966d-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="e966d-148">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="e966d-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e966d-149">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e966d-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e966d-150">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="e966d-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="e966d-151">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="e966d-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="e966d-152">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="e966d-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="e966d-153">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="e966d-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e966d-154">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="e966d-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="e966d-155">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e966d-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e966d-156">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e966d-156">Child elements</span></span>

|<span data-ttu-id="e966d-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e966d-157">**Element**</span></span>|<span data-ttu-id="e966d-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e966d-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e966d-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="e966d-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e966d-160">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="e966d-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e966d-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e966d-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e966d-162">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e966d-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e966d-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e966d-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e966d-164">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="e966d-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e966d-165">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="e966d-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e966d-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e966d-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e966d-167">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="e966d-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e966d-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="e966d-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="e966d-169">Contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e966d-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e966d-170">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e966d-170">Parent elements</span></span>

|<span data-ttu-id="e966d-171">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e966d-171">**Element**</span></span>|<span data-ttu-id="e966d-172">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e966d-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e966d-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e966d-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e966d-174">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e966d-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e966d-175">Comentários</span><span class="sxs-lookup"><span data-stu-id="e966d-175">Remarks</span></span>

<span data-ttu-id="e966d-176">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e966d-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e966d-177">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e966d-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e966d-178">Namespace</span><span class="sxs-lookup"><span data-stu-id="e966d-178">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e966d-179">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e966d-179">Schema Name</span></span>  <br/> |<span data-ttu-id="e966d-180">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e966d-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="e966d-181">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e966d-181">Validation File</span></span>  <br/> |<span data-ttu-id="e966d-182">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e966d-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e966d-183">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e966d-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="e966d-184">False</span><span class="sxs-lookup"><span data-stu-id="e966d-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e966d-185">Ver também</span><span class="sxs-lookup"><span data-stu-id="e966d-185">See also</span></span>

- [<span data-ttu-id="e966d-186">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="e966d-186">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="e966d-187">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="e966d-187">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="e966d-188">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e966d-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

