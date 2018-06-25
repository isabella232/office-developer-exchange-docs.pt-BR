---
title: GetSharingMetadataResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponse
api_type:
- schema
ms.assetid: 1acc2d8f-7104-4b36-9c04-dd4fc4f571bb
description: O elemento de GetSharingMetadataResponse define uma resposta a uma solicitação de operação GetSharingMetadata.
ms.openlocfilehash: 820b5bf7aa5528b61aa6649e5b1886885b5f022e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823676"
---
# <a name="getsharingmetadataresponse"></a><span data-ttu-id="b6864-103">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="b6864-103">GetSharingMetadataResponse</span></span>

<span data-ttu-id="b6864-104">O elemento de **GetSharingMetadataResponse** define uma resposta a uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b6864-104">The **GetSharingMetadataResponse** element defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponse>
```

 <span data-ttu-id="b6864-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b6864-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6864-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b6864-106">Attributes and elements</span></span>

<span data-ttu-id="b6864-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b6864-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6864-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b6864-108">Attributes</span></span>

|<span data-ttu-id="b6864-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="b6864-109">**Attribute**</span></span>|<span data-ttu-id="b6864-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6864-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6864-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b6864-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b6864-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6864-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b6864-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="b6864-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b6864-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="b6864-114">-  Success</span></span>  <br/><span data-ttu-id="b6864-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="b6864-115">-  Warning</span></span>  <br/><span data-ttu-id="b6864-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="b6864-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b6864-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b6864-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b6864-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b6864-118">**Value**</span></span>|<span data-ttu-id="b6864-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6864-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6864-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="b6864-120">**Success**</span></span> <br/> |<span data-ttu-id="b6864-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="b6864-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b6864-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b6864-122">**Warning**</span></span> <br/> | <span data-ttu-id="b6864-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="b6864-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b6864-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="b6864-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b6864-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="b6864-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b6864-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="b6864-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b6864-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="b6864-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="b6864-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="b6864-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b6864-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="b6864-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b6864-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="b6864-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b6864-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="b6864-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b6864-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="b6864-132">**Error**</span></span> <br/> | <span data-ttu-id="b6864-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="b6864-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b6864-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="b6864-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b6864-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b6864-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b6864-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="b6864-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b6864-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="b6864-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="b6864-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="b6864-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b6864-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="b6864-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b6864-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="b6864-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="b6864-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b6864-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b6864-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b6864-142">Child elements</span></span>

|<span data-ttu-id="b6864-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6864-143">**Element**</span></span>|<span data-ttu-id="b6864-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6864-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6864-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b6864-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b6864-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6864-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b6864-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b6864-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b6864-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6864-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b6864-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b6864-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b6864-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="b6864-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b6864-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="b6864-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b6864-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b6864-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b6864-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="b6864-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b6864-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="b6864-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="b6864-155">Contém uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.</span><span class="sxs-lookup"><span data-stu-id="b6864-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="b6864-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="b6864-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="b6864-157">Representa os destinatários da pasta de solicitação de compartilhamento que são inválidos.</span><span class="sxs-lookup"><span data-stu-id="b6864-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6864-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b6864-158">Parent elements</span></span>

<span data-ttu-id="b6864-159">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b6864-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6864-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="b6864-160">Remarks</span></span>

<span data-ttu-id="b6864-161">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b6864-161">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6864-162">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b6864-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6864-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6864-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b6864-164">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b6864-164">Schema Name</span></span>  <br/> |<span data-ttu-id="b6864-165">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b6864-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b6864-166">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b6864-166">Validation File</span></span>  <br/> |<span data-ttu-id="b6864-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b6864-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b6864-168">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b6864-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6864-169">False</span><span class="sxs-lookup"><span data-stu-id="b6864-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6864-170">Ver também</span><span class="sxs-lookup"><span data-stu-id="b6864-170">See also</span></span>

- [<span data-ttu-id="b6864-171">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="b6864-171">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="b6864-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6864-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

