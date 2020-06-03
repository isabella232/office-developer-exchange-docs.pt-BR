---
title: CopyItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: O elemento CopyItemResponseMessage contém o status e o resultado de uma única solicitação de operação de CopyItem.
ms.openlocfilehash: 99449a4c05d0b2ea13dfca4235aa5f40d54d1214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466441"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="68769-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="68769-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="68769-104">O elemento **CopyItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="68769-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="68769-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="68769-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68769-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="68769-106">Attributes and elements</span></span>

<span data-ttu-id="68769-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="68769-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68769-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="68769-108">Attributes</span></span>

|<span data-ttu-id="68769-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="68769-109">**Attribute**</span></span>|<span data-ttu-id="68769-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68769-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68769-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="68769-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="68769-112">Descreve o status de uma resposta de [operação do CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="68769-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="68769-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="68769-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="68769-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="68769-114">- Success</span></span>  <br/><span data-ttu-id="68769-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="68769-115">-  Warning</span></span>  <br/><span data-ttu-id="68769-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="68769-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="68769-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="68769-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="68769-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="68769-118">**Value**</span></span>|<span data-ttu-id="68769-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68769-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68769-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="68769-120">**Success**</span></span> <br/> |<span data-ttu-id="68769-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="68769-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="68769-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="68769-122">**Warning**</span></span> <br/> | <span data-ttu-id="68769-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="68769-123">Describes a request that was not processed.</span></span> <span data-ttu-id="68769-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="68769-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="68769-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="68769-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="68769-126">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="68769-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="68769-127">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="68769-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="68769-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="68769-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="68769-129">– O banco de dados de caixa de correio (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="68769-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="68769-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="68769-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="68769-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="68769-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="68769-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="68769-132">**Error**</span></span> <br/> | <span data-ttu-id="68769-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="68769-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="68769-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="68769-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="68769-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="68769-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="68769-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="68769-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="68769-137">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="68769-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="68769-138">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="68769-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="68769-139">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="68769-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="68769-140">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="68769-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="68769-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="68769-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="68769-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="68769-142">Child elements</span></span>

|<span data-ttu-id="68769-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68769-143">**Element**</span></span>|<span data-ttu-id="68769-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68769-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68769-145">- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="68769-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="68769-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="68769-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="68769-147">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="68769-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="68769-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68769-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="68769-149">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="68769-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="68769-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="68769-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="68769-151">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="68769-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="68769-152">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="68769-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="68769-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="68769-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="68769-154">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="68769-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="68769-155">Itens</span><span class="sxs-lookup"><span data-stu-id="68769-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="68769-156">Contém uma matriz de itens copiados</span><span class="sxs-lookup"><span data-stu-id="68769-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68769-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="68769-157">Parent elements</span></span>

|<span data-ttu-id="68769-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68769-158">**Element**</span></span>|<span data-ttu-id="68769-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68769-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68769-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="68769-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="68769-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="68769-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68769-162">Comentários</span><span class="sxs-lookup"><span data-stu-id="68769-162">Remarks</span></span>

<span data-ttu-id="68769-163">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="68769-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68769-164">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="68769-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68769-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="68769-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68769-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="68769-166">Schema name</span></span>  <br/> |<span data-ttu-id="68769-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="68769-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68769-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="68769-168">Validation file</span></span>  <br/> |<span data-ttu-id="68769-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68769-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68769-170">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="68769-170">Can be empty</span></span>  <br/> |<span data-ttu-id="68769-171">False</span><span class="sxs-lookup"><span data-stu-id="68769-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68769-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="68769-172">See also</span></span>

- [<span data-ttu-id="68769-173">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="68769-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="68769-174">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="68769-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

