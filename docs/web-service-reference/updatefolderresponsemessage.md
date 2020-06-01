---
title: UpdateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponseMessage
api_type:
- schema
ms.assetid: 914bb683-49ee-44a2-b59d-ef560244dfb8
description: O elemento UpdateFolderResponseMessage contém o status e o resultado de atualizações definidas pelo elemento FolderChange de uma solicitação de operação UpdateFolder.
ms.openlocfilehash: bbe01583072e6203e099d440f2a171012f51e7df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466581"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="b79cc-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b79cc-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="b79cc-104">O elemento **UpdateFolderResponseMessage** contém o status e o resultado de atualizações definidas pelo elemento [FolderChange](folderchange.md) de uma solicitação de [operação UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b79cc-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b79cc-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b79cc-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="b79cc-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b79cc-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b79cc-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b79cc-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="b79cc-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b79cc-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b79cc-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b79cc-109">Attributes and elements</span></span>

<span data-ttu-id="b79cc-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b79cc-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b79cc-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="b79cc-111">Attributes</span></span>

|<span data-ttu-id="b79cc-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b79cc-112">**Attribute**</span></span>|<span data-ttu-id="b79cc-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b79cc-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b79cc-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b79cc-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b79cc-115">Descreve o status de uma resposta de [operação do UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b79cc-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b79cc-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="b79cc-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b79cc-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="b79cc-117">-  Success</span></span>  <br/><span data-ttu-id="b79cc-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="b79cc-118">-  Warning</span></span>  <br/><span data-ttu-id="b79cc-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="b79cc-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b79cc-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b79cc-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="b79cc-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b79cc-121">**Value**</span></span>|<span data-ttu-id="b79cc-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b79cc-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b79cc-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="b79cc-123">**Success**</span></span> <br/> |<span data-ttu-id="b79cc-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="b79cc-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b79cc-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="b79cc-125">**Warning**</span></span> <br/> | <span data-ttu-id="b79cc-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="b79cc-126">Describes a request that was not processed.</span></span> <span data-ttu-id="b79cc-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="b79cc-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b79cc-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="b79cc-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b79cc-129">– O repositório do Exchange está offline.</span><span class="sxs-lookup"><span data-stu-id="b79cc-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="b79cc-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="b79cc-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b79cc-131">-Uma caixa de correio é movida.</span><span class="sxs-lookup"><span data-stu-id="b79cc-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="b79cc-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="b79cc-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="b79cc-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="b79cc-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b79cc-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="b79cc-134">**Error**</span></span> <br/> | <span data-ttu-id="b79cc-135">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="b79cc-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b79cc-136">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="b79cc-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="b79cc-137">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="b79cc-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b79cc-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="b79cc-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b79cc-139">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="b79cc-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="b79cc-140">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="b79cc-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b79cc-141">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="b79cc-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b79cc-142">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="b79cc-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="b79cc-143">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b79cc-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b79cc-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b79cc-144">Child elements</span></span>

|<span data-ttu-id="b79cc-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b79cc-145">**Element**</span></span>|<span data-ttu-id="b79cc-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b79cc-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b79cc-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="b79cc-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b79cc-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b79cc-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b79cc-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b79cc-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b79cc-150">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="b79cc-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b79cc-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b79cc-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b79cc-152">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="b79cc-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b79cc-153">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="b79cc-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b79cc-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b79cc-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b79cc-155">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="b79cc-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b79cc-156">Pastas</span><span class="sxs-lookup"><span data-stu-id="b79cc-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b79cc-157">Contém uma matriz de pastas usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="b79cc-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b79cc-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b79cc-158">Parent elements</span></span>

|<span data-ttu-id="b79cc-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b79cc-159">**Element**</span></span>|<span data-ttu-id="b79cc-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b79cc-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b79cc-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b79cc-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b79cc-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b79cc-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b79cc-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="b79cc-163">Remarks</span></span>

<span data-ttu-id="b79cc-164">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b79cc-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b79cc-165">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b79cc-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b79cc-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="b79cc-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b79cc-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b79cc-167">Schema Name</span></span>  <br/> |<span data-ttu-id="b79cc-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b79cc-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b79cc-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b79cc-169">Validation File</span></span>  <br/> |<span data-ttu-id="b79cc-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b79cc-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b79cc-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b79cc-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="b79cc-172">False</span><span class="sxs-lookup"><span data-stu-id="b79cc-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b79cc-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="b79cc-173">See also</span></span>

- [<span data-ttu-id="b79cc-174">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="b79cc-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

