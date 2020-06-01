---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: O elemento FindItemResponseMessage contém o status e o resultado de uma única solicitação de operação de FindItem.
ms.openlocfilehash: ca941e0c7e5b9b08f6f495ccae0d634d72b8f429
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462532"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="d483e-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d483e-103">FindItemResponseMessage</span></span>

<span data-ttu-id="d483e-104">O elemento **FindItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d483e-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d483e-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="d483e-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="d483e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d483e-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d483e-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d483e-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="d483e-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d483e-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d483e-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d483e-109">Attributes and elements</span></span>

<span data-ttu-id="d483e-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d483e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d483e-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="d483e-111">Attributes</span></span>

|<span data-ttu-id="d483e-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d483e-112">**Attribute**</span></span>|<span data-ttu-id="d483e-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d483e-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d483e-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d483e-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d483e-115">Descreve o status de uma resposta de [operação do FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d483e-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="d483e-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="d483e-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="d483e-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="d483e-117">-  Success</span></span>  <br/><span data-ttu-id="d483e-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="d483e-118">-  Warning</span></span>  <br/><span data-ttu-id="d483e-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="d483e-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d483e-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d483e-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d483e-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d483e-121">**Value**</span></span>|<span data-ttu-id="d483e-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d483e-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d483e-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="d483e-123">**Success**</span></span> <br/> |<span data-ttu-id="d483e-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="d483e-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d483e-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="d483e-125">**Warning**</span></span> <br/> | <span data-ttu-id="d483e-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="d483e-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d483e-127">Um aviso pode ser retornado se ocorreu um erro ao processar um item na solicitação, o processamento e os itens subsequentes não puderam ser processados.</span><span class="sxs-lookup"><span data-stu-id="d483e-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d483e-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="d483e-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="d483e-129">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="d483e-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="d483e-130">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="d483e-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="d483e-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="d483e-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d483e-132">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="d483e-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="d483e-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="d483e-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="d483e-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="d483e-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="d483e-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="d483e-135">**Error**</span></span> <br/> | <span data-ttu-id="d483e-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="d483e-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d483e-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="d483e-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d483e-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="d483e-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d483e-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="d483e-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d483e-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="d483e-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="d483e-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="d483e-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d483e-142">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="d483e-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d483e-143">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="d483e-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d483e-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d483e-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d483e-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d483e-145">Child elements</span></span>

|<span data-ttu-id="d483e-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d483e-146">**Element**</span></span>|<span data-ttu-id="d483e-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d483e-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d483e-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d483e-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d483e-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="d483e-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d483e-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d483e-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d483e-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="d483e-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d483e-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d483e-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d483e-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="d483e-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d483e-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="d483e-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d483e-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d483e-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d483e-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="d483e-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d483e-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d483e-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="d483e-158">Contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d483e-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d483e-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d483e-159">Parent elements</span></span>

|<span data-ttu-id="d483e-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d483e-160">**Element**</span></span>|<span data-ttu-id="d483e-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d483e-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d483e-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d483e-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d483e-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d483e-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d483e-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="d483e-164">Remarks</span></span>

<span data-ttu-id="d483e-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d483e-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d483e-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d483e-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d483e-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="d483e-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d483e-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d483e-168">Schema name</span></span>  <br/> |<span data-ttu-id="d483e-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d483e-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d483e-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d483e-170">Validation file</span></span>  <br/> |<span data-ttu-id="d483e-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d483e-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d483e-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d483e-172">Can be empty</span></span>  <br/> |<span data-ttu-id="d483e-173">False</span><span class="sxs-lookup"><span data-stu-id="d483e-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d483e-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="d483e-174">See also</span></span>

- [<span data-ttu-id="d483e-175">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="d483e-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="d483e-176">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="d483e-176">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

