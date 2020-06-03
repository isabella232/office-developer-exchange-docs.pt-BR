---
title: GetSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponse
api_type:
- schema
ms.assetid: fee90e84-3ad4-4c4b-831f-bbc95070aebf
description: O elemento GetSharingFolderResponse define uma resposta a uma solicitação de operação GetSharingFolder.
ms.openlocfilehash: 2b5a263b350ae54e87a8fea7cb7cc2d9485b5814
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460481"
---
# <a name="getsharingfolderresponse"></a><span data-ttu-id="9d4c5-103">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="9d4c5-103">GetSharingFolderResponse</span></span>

<span data-ttu-id="9d4c5-104">O elemento **GetSharingFolderResponse** define uma resposta a uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9d4c5-104">The **GetSharingFolderResponse** element defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```XML
<GetSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponse>
```

 <span data-ttu-id="9d4c5-105">**GetSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d4c5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9d4c5-106">Attributes and elements</span></span>

<span data-ttu-id="9d4c5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d4c5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d4c5-108">Attributes</span></span>

|<span data-ttu-id="9d4c5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-109">**Attribute**</span></span>|<span data-ttu-id="9d4c5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9d4c5-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9d4c5-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="9d4c5-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="9d4c5-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="9d4c5-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="9d4c5-114">-  Success</span></span>  <br/><span data-ttu-id="9d4c5-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="9d4c5-115">-  Warning</span></span>  <br/><span data-ttu-id="9d4c5-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="9d4c5-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9d4c5-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9d4c5-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9d4c5-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-118">**Value**</span></span>|<span data-ttu-id="9d4c5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9d4c5-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-120">**Success**</span></span> <br/> |<span data-ttu-id="9d4c5-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9d4c5-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-122">**Warning**</span></span> <br/> | <span data-ttu-id="9d4c5-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9d4c5-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9d4c5-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="9d4c5-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9d4c5-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9d4c5-127">– O serviço de diretório do Active Directory ou o AD DS (serviços de domínio Active Directory) está offline.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-127">-  The Active Directory directory service or Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9d4c5-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9d4c5-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9d4c5-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9d4c5-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9d4c5-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-132">**Error**</span></span> <br/> | <span data-ttu-id="9d4c5-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9d4c5-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="9d4c5-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9d4c5-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="9d4c5-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9d4c5-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="9d4c5-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9d4c5-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="9d4c5-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="9d4c5-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="9d4c5-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9d4c5-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="9d4c5-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9d4c5-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="9d4c5-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9d4c5-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9d4c5-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9d4c5-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d4c5-142">Child elements</span></span>

|<span data-ttu-id="9d4c5-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-143">**Element**</span></span>|<span data-ttu-id="9d4c5-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d4c5-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d4c5-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9d4c5-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9d4c5-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9d4c5-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9d4c5-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9d4c5-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9d4c5-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9d4c5-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9d4c5-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="9d4c5-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9d4c5-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9d4c5-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9d4c5-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9d4c5-154">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="9d4c5-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="9d4c5-155">Representa o identificador da pasta local em uma relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d4c5-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d4c5-156">Parent elements</span></span>

<span data-ttu-id="9d4c5-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d4c5-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d4c5-158">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d4c5-158">Remarks</span></span>

<span data-ttu-id="9d4c5-159">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d4c5-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d4c5-160">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9d4c5-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d4c5-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d4c5-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d4c5-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d4c5-162">Schema Name</span></span>  <br/> |<span data-ttu-id="9d4c5-163">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9d4c5-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d4c5-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d4c5-164">Validation File</span></span>  <br/> |<span data-ttu-id="9d4c5-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d4c5-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d4c5-166">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d4c5-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d4c5-167">False</span><span class="sxs-lookup"><span data-stu-id="9d4c5-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d4c5-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="9d4c5-168">See also</span></span>

- [<span data-ttu-id="9d4c5-169">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d4c5-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

