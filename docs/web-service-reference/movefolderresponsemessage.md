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
description: O elemento MoveFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de MoveFolder.
ms.openlocfilehash: 634fec89445b49d1c8c42541f2fc50d07b5a1acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467470"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="86055-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="86055-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="86055-104">O elemento **MoveFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="86055-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="86055-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="86055-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="86055-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="86055-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="86055-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="86055-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="86055-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="86055-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86055-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="86055-109">Attributes and elements</span></span>

<span data-ttu-id="86055-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="86055-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86055-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="86055-111">Attributes</span></span>

|<span data-ttu-id="86055-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="86055-112">**Attribute**</span></span>|<span data-ttu-id="86055-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86055-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="86055-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="86055-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="86055-115">Descreve o status de uma resposta de [operação do MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="86055-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="86055-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="86055-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="86055-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="86055-117">-  Success</span></span>  <br/><span data-ttu-id="86055-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="86055-118">-  Warning</span></span>  <br/><span data-ttu-id="86055-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="86055-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="86055-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="86055-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="86055-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="86055-121">**Value**</span></span>|<span data-ttu-id="86055-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86055-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="86055-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="86055-123">**Success**</span></span> <br/> |<span data-ttu-id="86055-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="86055-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="86055-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="86055-125">**Warning**</span></span> <br/> | <span data-ttu-id="86055-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="86055-126">Describes a request that was not processed.</span></span> <span data-ttu-id="86055-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="86055-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="86055-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="86055-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="86055-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="86055-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="86055-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="86055-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="86055-131">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="86055-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="86055-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="86055-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="86055-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="86055-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="86055-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="86055-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="86055-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="86055-135">**Error**</span></span> <br/> | <span data-ttu-id="86055-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="86055-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="86055-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="86055-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="86055-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="86055-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="86055-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="86055-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="86055-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="86055-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="86055-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="86055-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="86055-142">– Qualquer tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="86055-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="86055-143">-Qualquer falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="86055-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="86055-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="86055-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="86055-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="86055-145">Child elements</span></span>

|<span data-ttu-id="86055-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="86055-146">**Element**</span></span>|<span data-ttu-id="86055-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86055-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86055-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="86055-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="86055-149">Uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="86055-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="86055-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="86055-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="86055-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="86055-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="86055-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="86055-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="86055-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="86055-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="86055-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="86055-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="86055-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="86055-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="86055-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="86055-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="86055-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="86055-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="86055-158">Contém uma matriz de pastas movidas.</span><span class="sxs-lookup"><span data-stu-id="86055-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86055-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="86055-159">Parent elements</span></span>

|<span data-ttu-id="86055-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="86055-160">**Element**</span></span>|<span data-ttu-id="86055-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86055-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86055-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="86055-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="86055-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="86055-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86055-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="86055-164">Remarks</span></span>

<span data-ttu-id="86055-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="86055-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86055-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="86055-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86055-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="86055-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86055-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="86055-168">Schema Name</span></span>  <br/> |<span data-ttu-id="86055-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="86055-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86055-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="86055-170">Validation File</span></span>  <br/> |<span data-ttu-id="86055-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86055-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86055-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="86055-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="86055-173">False</span><span class="sxs-lookup"><span data-stu-id="86055-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86055-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="86055-174">See also</span></span>

- [<span data-ttu-id="86055-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="86055-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="86055-176">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="86055-176">MoveFolder operation</span></span>](movefolder-operation.md)

