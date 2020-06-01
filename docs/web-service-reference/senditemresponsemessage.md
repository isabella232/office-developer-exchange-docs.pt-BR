---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: O elemento SendItemResponseMessage contém o status e o resultado de uma única solicitação de operação de SendItem.
ms.openlocfilehash: fc5d4f6dc77b242c3d3d517133c23ed56956c1ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462266"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="1a292-103">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1a292-103">SendItemResponseMessage</span></span>

<span data-ttu-id="1a292-104">O elemento **SendItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1a292-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="1a292-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1a292-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a292-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1a292-106">Attributes and elements</span></span>

<span data-ttu-id="1a292-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1a292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a292-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1a292-108">Attributes</span></span>

|<span data-ttu-id="1a292-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="1a292-109">**Attribute**</span></span>|<span data-ttu-id="1a292-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a292-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a292-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1a292-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1a292-112">Descreve o status de uma resposta de [operação do SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1a292-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="1a292-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="1a292-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="1a292-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="1a292-114">-  Success</span></span>  <br/><span data-ttu-id="1a292-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="1a292-115">-  Warning</span></span>  <br/><span data-ttu-id="1a292-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="1a292-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1a292-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1a292-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1a292-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="1a292-118">**Value**</span></span>|<span data-ttu-id="1a292-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a292-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a292-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="1a292-120">**Success**</span></span> <br/> |<span data-ttu-id="1a292-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="1a292-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1a292-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="1a292-122">**Warning**</span></span> <br/> | <span data-ttu-id="1a292-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="1a292-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1a292-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="1a292-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1a292-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="1a292-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1a292-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="1a292-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1a292-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="1a292-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1a292-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="1a292-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="1a292-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="1a292-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1a292-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="1a292-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1a292-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="1a292-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="1a292-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="1a292-132">**Error**</span></span> <br/> | <span data-ttu-id="1a292-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="1a292-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1a292-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="1a292-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="1a292-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="1a292-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1a292-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="1a292-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1a292-137">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="1a292-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="1a292-138">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="1a292-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1a292-139">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="1a292-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1a292-140">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="1a292-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="1a292-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1a292-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1a292-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1a292-142">Child elements</span></span>

|<span data-ttu-id="1a292-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a292-143">**Element**</span></span>|<span data-ttu-id="1a292-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a292-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a292-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1a292-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1a292-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a292-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1a292-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1a292-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1a292-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="1a292-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1a292-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1a292-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1a292-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="1a292-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1a292-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="1a292-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1a292-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1a292-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1a292-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="1a292-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a292-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1a292-154">Parent elements</span></span>

|<span data-ttu-id="1a292-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a292-155">**Element**</span></span>|<span data-ttu-id="1a292-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a292-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a292-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1a292-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1a292-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a292-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a292-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="1a292-159">Remarks</span></span>

<span data-ttu-id="1a292-160">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1a292-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a292-161">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1a292-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a292-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a292-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a292-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1a292-163">Schema Name</span></span>  <br/> |<span data-ttu-id="1a292-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1a292-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a292-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1a292-165">Validation File</span></span>  <br/> |<span data-ttu-id="1a292-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a292-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a292-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1a292-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a292-168">False</span><span class="sxs-lookup"><span data-stu-id="1a292-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a292-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a292-169">See also</span></span>

- [<span data-ttu-id="1a292-170">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="1a292-170">SendItem operation</span></span>](senditem-operation.md)
- [<span data-ttu-id="1a292-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1a292-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

