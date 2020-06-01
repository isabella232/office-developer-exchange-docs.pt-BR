---
title: UpdateInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: O elemento UpdateInboxRulesResponse define uma resposta a uma solicitação UpdateInboxRules.
ms.openlocfilehash: 1216a32bdaf2dd5211021add0728844eb62089ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455902"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="91700-103">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="91700-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="91700-104">O elemento **UpdateInboxRulesResponse** define uma resposta a uma solicitação UpdateInboxRules.</span><span class="sxs-lookup"><span data-stu-id="91700-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="91700-105">**UpdateInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="91700-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91700-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="91700-106">Attributes and elements</span></span>

<span data-ttu-id="91700-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91700-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91700-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91700-108">Attributes</span></span>

|<span data-ttu-id="91700-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="91700-109">**Attribute**</span></span>|<span data-ttu-id="91700-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91700-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91700-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="91700-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="91700-112">Descreve o status de uma resposta de [operação de cancelamento de assinatura](unsubscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="91700-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="91700-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="91700-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="91700-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="91700-114">-  Success</span></span>  <br/><span data-ttu-id="91700-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="91700-115">-  Warning</span></span>  <br/><span data-ttu-id="91700-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="91700-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="91700-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="91700-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="91700-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="91700-118">**Value**</span></span>|<span data-ttu-id="91700-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91700-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91700-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="91700-120">**Success**</span></span> <br/> |<span data-ttu-id="91700-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="91700-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="91700-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="91700-122">**Warning**</span></span> <br/> | <span data-ttu-id="91700-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="91700-123">Describes a request that was not processed.</span></span> <span data-ttu-id="91700-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="91700-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="91700-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="91700-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="91700-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="91700-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="91700-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="91700-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="91700-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="91700-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="91700-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="91700-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="91700-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="91700-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="91700-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="91700-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="91700-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="91700-132">**Error**</span></span> <br/> | <span data-ttu-id="91700-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="91700-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="91700-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="91700-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="91700-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="91700-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="91700-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="91700-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="91700-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="91700-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="91700-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="91700-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="91700-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="91700-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="91700-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="91700-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="91700-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="91700-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="91700-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91700-142">Child elements</span></span>

|<span data-ttu-id="91700-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="91700-143">**Element**</span></span>|<span data-ttu-id="91700-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91700-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91700-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="91700-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="91700-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="91700-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="91700-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="91700-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="91700-148">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="91700-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="91700-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="91700-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="91700-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="91700-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="91700-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="91700-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="91700-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="91700-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="91700-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="91700-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="91700-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="91700-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="91700-155">Representa uma matriz de erros de validação de regra em cada campo de regra que possui um erro.</span><span class="sxs-lookup"><span data-stu-id="91700-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="91700-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91700-156">Parent elements</span></span>

<span data-ttu-id="91700-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91700-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="91700-158">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="91700-158">Text value</span></span>

<span data-ttu-id="91700-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91700-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91700-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="91700-160">Remarks</span></span>

<span data-ttu-id="91700-161">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91700-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91700-162">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="91700-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91700-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="91700-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="91700-164">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91700-164">Schema name</span></span>  <br/> |<span data-ttu-id="91700-165">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="91700-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="91700-166">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91700-166">Validation file</span></span>  <br/> |<span data-ttu-id="91700-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="91700-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="91700-168">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="91700-168">Can be empty</span></span>  <br/> |<span data-ttu-id="91700-169">False</span><span class="sxs-lookup"><span data-stu-id="91700-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91700-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="91700-170">See also</span></span>

- [<span data-ttu-id="91700-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="91700-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="91700-172">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="91700-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="91700-173">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="91700-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

