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
description: O elemento UpdateFolderResponseMessage contém o status e o resultado de atualizações definido pelo elemento FolderChange de uma solicitação de operação UpdateFolder.
ms.openlocfilehash: 4cd00232bcc233f6534d844418f523c248ce54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837900"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="04d42-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04d42-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="04d42-104">O elemento **UpdateFolderResponseMessage** contém o status e o resultado de atualizações definido pelo elemento [FolderChange](folderchange.md) de uma solicitação de [operação UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="04d42-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="04d42-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="04d42-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="04d42-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="04d42-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="04d42-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="04d42-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="04d42-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="04d42-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04d42-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="04d42-109">Attributes and elements</span></span>

<span data-ttu-id="04d42-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="04d42-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04d42-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="04d42-111">Attributes</span></span>

|<span data-ttu-id="04d42-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="04d42-112">**Attribute**</span></span>|<span data-ttu-id="04d42-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04d42-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04d42-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="04d42-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="04d42-115">Descreve o status de uma resposta [UpdateFolder operação](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="04d42-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="04d42-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="04d42-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="04d42-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="04d42-117">-  Success</span></span>  <br/><span data-ttu-id="04d42-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="04d42-118">-  Warning</span></span>  <br/><span data-ttu-id="04d42-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="04d42-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="04d42-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="04d42-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="04d42-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="04d42-121">**Value**</span></span>|<span data-ttu-id="04d42-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04d42-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04d42-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="04d42-123">**Success**</span></span> <br/> |<span data-ttu-id="04d42-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="04d42-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="04d42-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="04d42-125">**Warning**</span></span> <br/> | <span data-ttu-id="04d42-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="04d42-126">Describes a request that was not processed.</span></span> <span data-ttu-id="04d42-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="04d42-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="04d42-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="04d42-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="04d42-129">-O armazenamento do Exchange está offline.</span><span class="sxs-lookup"><span data-stu-id="04d42-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="04d42-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="04d42-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="04d42-131">-Uma caixa de correio é movida.</span><span class="sxs-lookup"><span data-stu-id="04d42-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="04d42-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="04d42-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="04d42-133">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="04d42-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="04d42-134">**Erro**</span><span class="sxs-lookup"><span data-stu-id="04d42-134">**Error**</span></span> <br/> | <span data-ttu-id="04d42-135">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="04d42-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="04d42-136">Estes são exemplos de fontes para erros:</span><span class="sxs-lookup"><span data-stu-id="04d42-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="04d42-137">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="04d42-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="04d42-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="04d42-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="04d42-139">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="04d42-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="04d42-140">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="04d42-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="04d42-141">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="04d42-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="04d42-142">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="04d42-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="04d42-143">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="04d42-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="04d42-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="04d42-144">Child elements</span></span>

|<span data-ttu-id="04d42-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04d42-145">**Element**</span></span>|<span data-ttu-id="04d42-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04d42-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04d42-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="04d42-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="04d42-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="04d42-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="04d42-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="04d42-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="04d42-150">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="04d42-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="04d42-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="04d42-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="04d42-152">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="04d42-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="04d42-153">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="04d42-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="04d42-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="04d42-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="04d42-155">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="04d42-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="04d42-156">Pastas</span><span class="sxs-lookup"><span data-stu-id="04d42-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="04d42-157">Contém uma matriz de pastas usados nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="04d42-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04d42-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="04d42-158">Parent elements</span></span>

|<span data-ttu-id="04d42-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04d42-159">**Element**</span></span>|<span data-ttu-id="04d42-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04d42-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04d42-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="04d42-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="04d42-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="04d42-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04d42-163">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="04d42-163">Remarks</span></span>

<span data-ttu-id="04d42-164">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="04d42-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04d42-165">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="04d42-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04d42-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="04d42-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04d42-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="04d42-167">Schema Name</span></span>  <br/> |<span data-ttu-id="04d42-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="04d42-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04d42-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="04d42-169">Validation File</span></span>  <br/> |<span data-ttu-id="04d42-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04d42-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04d42-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="04d42-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="04d42-172">False</span><span class="sxs-lookup"><span data-stu-id="04d42-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04d42-173">Ver também</span><span class="sxs-lookup"><span data-stu-id="04d42-173">See also</span></span>

- [<span data-ttu-id="04d42-174">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="04d42-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

