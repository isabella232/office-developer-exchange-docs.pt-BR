---
title: MoveFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: O elemento MoveFolderResponseMessage contém o status e o resultado de uma única solicitação de operação MoveFolder.
ms.openlocfilehash: 777520bf6a093882da95a7bfd466b66acdab957c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824496"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="56832-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="56832-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="56832-104">O elemento **MoveFolderResponseMessage** contém o status e o resultado de uma única [operação MoveFolder](movefolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="56832-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="56832-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="56832-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="56832-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="56832-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="56832-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="56832-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="56832-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="56832-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56832-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="56832-109">Attributes and elements</span></span>

<span data-ttu-id="56832-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="56832-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56832-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="56832-111">Attributes</span></span>

|<span data-ttu-id="56832-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="56832-112">**Attribute**</span></span>|<span data-ttu-id="56832-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56832-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56832-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="56832-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="56832-115">Descreve o status de uma resposta [MoveFolder operação](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="56832-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="56832-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="56832-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="56832-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="56832-117">-  Success</span></span>  <br/><span data-ttu-id="56832-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="56832-118">-  Warning</span></span>  <br/><span data-ttu-id="56832-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="56832-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="56832-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="56832-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="56832-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="56832-121">**Value**</span></span>|<span data-ttu-id="56832-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56832-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56832-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="56832-123">**Success**</span></span> <br/> |<span data-ttu-id="56832-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="56832-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="56832-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="56832-125">**Warning**</span></span> <br/> | <span data-ttu-id="56832-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="56832-126">Describes a request that was not processed.</span></span> <span data-ttu-id="56832-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="56832-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="56832-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="56832-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="56832-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="56832-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="56832-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="56832-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="56832-131">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="56832-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="56832-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="56832-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="56832-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="56832-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="56832-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="56832-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="56832-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="56832-135">**Error**</span></span> <br/> | <span data-ttu-id="56832-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="56832-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="56832-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="56832-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="56832-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="56832-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="56832-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="56832-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="56832-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="56832-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="56832-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="56832-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="56832-142">-Qualquer tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="56832-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="56832-143">-Qualquer falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="56832-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="56832-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="56832-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="56832-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="56832-145">Child elements</span></span>

|<span data-ttu-id="56832-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="56832-146">**Element**</span></span>|<span data-ttu-id="56832-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56832-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56832-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="56832-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="56832-149">Uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="56832-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="56832-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="56832-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="56832-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="56832-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="56832-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="56832-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="56832-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="56832-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="56832-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="56832-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="56832-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="56832-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="56832-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="56832-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="56832-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="56832-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="56832-158">Contém uma matriz das pastas movidas.</span><span class="sxs-lookup"><span data-stu-id="56832-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56832-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="56832-159">Parent elements</span></span>

|<span data-ttu-id="56832-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="56832-160">**Element**</span></span>|<span data-ttu-id="56832-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56832-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56832-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="56832-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="56832-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56832-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56832-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="56832-164">Remarks</span></span>

<span data-ttu-id="56832-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="56832-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56832-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="56832-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56832-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="56832-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56832-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="56832-168">Schema Name</span></span>  <br/> |<span data-ttu-id="56832-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="56832-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="56832-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="56832-170">Validation File</span></span>  <br/> |<span data-ttu-id="56832-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="56832-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56832-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="56832-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="56832-173">False</span><span class="sxs-lookup"><span data-stu-id="56832-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56832-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="56832-174">See also</span></span>

- [<span data-ttu-id="56832-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="56832-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="56832-176">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="56832-176">MoveFolder operation</span></span>](movefolder-operation.md)

