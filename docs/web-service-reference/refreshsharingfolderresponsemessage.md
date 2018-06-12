---
title: RefreshSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponseMessage
api_type:
- schema
ms.assetid: 53ee65bd-cf75-4e04-9b27-eff1b040ae82
description: O elemento RefreshSharingFolderResponseMessage contém o status e o resultado de uma única solicitação de operação RefreshSharingFolder.
ms.openlocfilehash: 9dbb66c294439f33a9307d51c03dd1cd127e95e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825052"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="097f8-103">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="097f8-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="097f8-104">O elemento **RefreshSharingFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="097f8-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="097f8-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="097f8-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="097f8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="097f8-106">Attributes and elements</span></span>

<span data-ttu-id="097f8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="097f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="097f8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="097f8-108">Attributes</span></span>

|<span data-ttu-id="097f8-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="097f8-109">**Attribute**</span></span>|<span data-ttu-id="097f8-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097f8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097f8-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="097f8-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="097f8-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="097f8-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="097f8-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="097f8-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="097f8-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="097f8-114">-  Success</span></span>  <br/><span data-ttu-id="097f8-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="097f8-115">-  Warning</span></span>  <br/><span data-ttu-id="097f8-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="097f8-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="097f8-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="097f8-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="097f8-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="097f8-118">**Value**</span></span>|<span data-ttu-id="097f8-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097f8-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097f8-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="097f8-120">**Success**</span></span> <br/> |<span data-ttu-id="097f8-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="097f8-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="097f8-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="097f8-122">**Warning**</span></span> <br/> | <span data-ttu-id="097f8-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="097f8-123">Describes a request that was not processed.</span></span> <span data-ttu-id="097f8-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="097f8-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="097f8-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="097f8-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="097f8-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="097f8-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="097f8-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="097f8-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="097f8-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="097f8-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="097f8-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="097f8-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="097f8-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="097f8-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="097f8-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="097f8-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="097f8-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="097f8-132">**Error**</span></span> <br/> | <span data-ttu-id="097f8-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="097f8-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="097f8-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="097f8-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="097f8-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="097f8-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="097f8-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="097f8-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="097f8-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="097f8-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="097f8-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="097f8-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="097f8-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="097f8-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="097f8-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="097f8-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="097f8-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="097f8-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="097f8-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="097f8-142">Child elements</span></span>

|<span data-ttu-id="097f8-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097f8-143">**Element**</span></span>|<span data-ttu-id="097f8-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097f8-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097f8-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="097f8-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="097f8-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="097f8-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="097f8-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="097f8-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="097f8-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="097f8-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="097f8-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="097f8-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="097f8-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="097f8-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="097f8-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="097f8-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="097f8-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="097f8-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="097f8-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="097f8-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="097f8-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="097f8-154">Parent elements</span></span>

|<span data-ttu-id="097f8-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097f8-155">**Element**</span></span>|<span data-ttu-id="097f8-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097f8-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097f8-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="097f8-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="097f8-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="097f8-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="097f8-159">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="097f8-159">Remarks</span></span>

<span data-ttu-id="097f8-160">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="097f8-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="097f8-161">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="097f8-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="097f8-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="097f8-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="097f8-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="097f8-163">Schema Name</span></span>  <br/> |<span data-ttu-id="097f8-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="097f8-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="097f8-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="097f8-165">Validation File</span></span>  <br/> |<span data-ttu-id="097f8-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="097f8-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="097f8-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="097f8-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="097f8-168">False</span><span class="sxs-lookup"><span data-stu-id="097f8-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="097f8-169">Ver também</span><span class="sxs-lookup"><span data-stu-id="097f8-169">See also</span></span>

- [<span data-ttu-id="097f8-170">Operação RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="097f8-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="097f8-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="097f8-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

