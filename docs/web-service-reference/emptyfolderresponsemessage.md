---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: O elemento EmptyFolderResponseMessage contém o status e o resultado de uma única solicitação de EmptyFolder.
ms.openlocfilehash: fd69df45d7e1d6538a977b79711baa769413ea66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526211"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="acab0-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="acab0-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="acab0-104">O elemento **EmptyFolderResponseMessage** contém o status e o resultado de uma única solicitação de [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="acab0-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="acab0-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="acab0-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="acab0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="acab0-106">Attributes and elements</span></span>

<span data-ttu-id="acab0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="acab0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acab0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="acab0-108">Attributes</span></span>

|<span data-ttu-id="acab0-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="acab0-109">**Attribute**</span></span>|<span data-ttu-id="acab0-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="acab0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="acab0-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="acab0-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="acab0-112">Descreve o status de uma resposta de [operação do EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="acab0-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="acab0-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="acab0-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="acab0-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="acab0-114">-  Success</span></span>  <br/><span data-ttu-id="acab0-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="acab0-115">-  Warning</span></span>  <br/><span data-ttu-id="acab0-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="acab0-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="acab0-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="acab0-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="acab0-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="acab0-118">**Value**</span></span>|<span data-ttu-id="acab0-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="acab0-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="acab0-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="acab0-120">**Success**</span></span> <br/> |<span data-ttu-id="acab0-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="acab0-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="acab0-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="acab0-122">**Warning**</span></span> <br/> | <span data-ttu-id="acab0-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="acab0-123">Describes a request that was not processed.</span></span> <span data-ttu-id="acab0-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="acab0-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="acab0-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="acab0-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="acab0-126">– O repositório do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="acab0-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="acab0-127">– O AD DS (serviços de domínio Active Directory) fica offline.</span><span class="sxs-lookup"><span data-stu-id="acab0-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="acab0-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="acab0-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="acab0-129">– O banco de dados de mensagens (MDB) fica offline.</span><span class="sxs-lookup"><span data-stu-id="acab0-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="acab0-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="acab0-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="acab0-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="acab0-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="acab0-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="acab0-132">**Error**</span></span> <br/> | <span data-ttu-id="acab0-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="acab0-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="acab0-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="acab0-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="acab0-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="acab0-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="acab0-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="acab0-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="acab0-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="acab0-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="acab0-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="acab0-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="acab0-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="acab0-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="acab0-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="acab0-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="acab0-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="acab0-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="acab0-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="acab0-142">Child elements</span></span>

|<span data-ttu-id="acab0-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="acab0-143">**Element**</span></span>|<span data-ttu-id="acab0-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="acab0-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acab0-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="acab0-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="acab0-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="acab0-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="acab0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="acab0-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="acab0-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="acab0-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="acab0-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="acab0-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="acab0-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="acab0-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="acab0-151">Ele contém o valor de 0.</span><span class="sxs-lookup"><span data-stu-id="acab0-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="acab0-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="acab0-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="acab0-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="acab0-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="acab0-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="acab0-154">Parent elements</span></span>

|<span data-ttu-id="acab0-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="acab0-155">**Element**</span></span>|<span data-ttu-id="acab0-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="acab0-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acab0-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="acab0-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="acab0-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="acab0-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="acab0-159">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="acab0-159">Text value</span></span>

<span data-ttu-id="acab0-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="acab0-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="acab0-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="acab0-161">Remarks</span></span>

<span data-ttu-id="acab0-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="acab0-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="acab0-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="acab0-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="acab0-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="acab0-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="acab0-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="acab0-165">Schema Name</span></span>  <br/> |<span data-ttu-id="acab0-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="acab0-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="acab0-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="acab0-167">Validation File</span></span>  <br/> |<span data-ttu-id="acab0-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="acab0-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="acab0-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="acab0-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="acab0-170">False</span><span class="sxs-lookup"><span data-stu-id="acab0-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acab0-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="acab0-171">See also</span></span>

- [<span data-ttu-id="acab0-172">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="acab0-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="acab0-173">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="acab0-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="acab0-174">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="acab0-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

