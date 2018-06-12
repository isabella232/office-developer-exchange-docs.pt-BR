---
title: RefreshSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: O elemento de RefreshSharingFolderResponse define uma resposta a uma solicitação de operação RefreshSharingFolder.
ms.openlocfilehash: 4ef7a63b2153c6106dae988439f499046689c2b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825048"
---
# <a name="refreshsharingfolderresponse"></a><span data-ttu-id="90ef6-103">RefreshSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="90ef6-103">RefreshSharingFolderResponse</span></span>

<span data-ttu-id="90ef6-104">O elemento de **RefreshSharingFolderResponse** define uma resposta a uma solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="90ef6-104">The **RefreshSharingFolderResponse** element defines a response to a [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 <span data-ttu-id="90ef6-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="90ef6-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90ef6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="90ef6-106">Attributes and elements</span></span>

<span data-ttu-id="90ef6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90ef6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90ef6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90ef6-108">Attributes</span></span>

|<span data-ttu-id="90ef6-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="90ef6-109">**Attribute**</span></span>|<span data-ttu-id="90ef6-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ef6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90ef6-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="90ef6-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="90ef6-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ef6-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="90ef6-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="90ef6-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="90ef6-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="90ef6-114">-  Success</span></span>  <br/><span data-ttu-id="90ef6-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="90ef6-115">-  Warning</span></span>  <br/><span data-ttu-id="90ef6-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="90ef6-116">-  Error</span></span>  <br/>- |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="90ef6-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="90ef6-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="90ef6-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="90ef6-118">**Value**</span></span>|<span data-ttu-id="90ef6-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ef6-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90ef6-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="90ef6-120">**Success**</span></span> <br/> |<span data-ttu-id="90ef6-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="90ef6-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="90ef6-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="90ef6-122">**Warning**</span></span> <br/> | <span data-ttu-id="90ef6-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="90ef6-123">Describes a request that was not processed.</span></span> <span data-ttu-id="90ef6-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="90ef6-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="90ef6-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="90ef6-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="90ef6-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="90ef6-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="90ef6-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="90ef6-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="90ef6-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="90ef6-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="90ef6-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="90ef6-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="90ef6-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="90ef6-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="90ef6-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="90ef6-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="90ef6-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="90ef6-132">**Error**</span></span> <br/> | <span data-ttu-id="90ef6-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="90ef6-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="90ef6-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="90ef6-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="90ef6-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="90ef6-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="90ef6-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="90ef6-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="90ef6-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="90ef6-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="90ef6-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="90ef6-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="90ef6-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="90ef6-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="90ef6-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="90ef6-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="90ef6-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="90ef6-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90ef6-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90ef6-142">Child elements</span></span>

|<span data-ttu-id="90ef6-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90ef6-143">**Element**</span></span>|<span data-ttu-id="90ef6-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ef6-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90ef6-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="90ef6-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="90ef6-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ef6-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="90ef6-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="90ef6-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="90ef6-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ef6-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="90ef6-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="90ef6-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="90ef6-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="90ef6-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="90ef6-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="90ef6-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="90ef6-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="90ef6-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="90ef6-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="90ef6-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90ef6-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90ef6-154">Parent elements</span></span>

<span data-ttu-id="90ef6-155">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90ef6-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90ef6-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="90ef6-156">Remarks</span></span>

<span data-ttu-id="90ef6-157">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="90ef6-157">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90ef6-158">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="90ef6-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90ef6-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="90ef6-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90ef6-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90ef6-160">Schema Name</span></span>  <br/> |<span data-ttu-id="90ef6-161">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="90ef6-161">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90ef6-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90ef6-162">Validation File</span></span>  <br/> |<span data-ttu-id="90ef6-163">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="90ef6-163">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90ef6-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90ef6-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="90ef6-165">False</span><span class="sxs-lookup"><span data-stu-id="90ef6-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90ef6-166">Ver também</span><span class="sxs-lookup"><span data-stu-id="90ef6-166">See also</span></span>

- [<span data-ttu-id="90ef6-167">Operação RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="90ef6-167">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="90ef6-168">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90ef6-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

