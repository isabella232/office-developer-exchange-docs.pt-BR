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
description: O elemento RefreshSharingFolderResponseMessage contém o status e o resultado de uma única solicitação de operação de RefreshSharingFolder.
ms.openlocfilehash: f2cc357298d523b418d2c45598639627c5a63252
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468667"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="1b82a-103">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1b82a-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="1b82a-104">O elemento **RefreshSharingFolderResponseMessage** contém o status e o resultado de uma única solicitação de [operação de RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1b82a-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="1b82a-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1b82a-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b82a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1b82a-106">Attributes and elements</span></span>

<span data-ttu-id="1b82a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1b82a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b82a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1b82a-108">Attributes</span></span>

|<span data-ttu-id="1b82a-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="1b82a-109">**Attribute**</span></span>|<span data-ttu-id="1b82a-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b82a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b82a-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1b82a-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1b82a-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b82a-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="1b82a-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="1b82a-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1b82a-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="1b82a-114">-  Success</span></span>  <br/><span data-ttu-id="1b82a-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="1b82a-115">-  Warning</span></span>  <br/><span data-ttu-id="1b82a-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="1b82a-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1b82a-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1b82a-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1b82a-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="1b82a-118">**Value**</span></span>|<span data-ttu-id="1b82a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b82a-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b82a-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="1b82a-120">**Success**</span></span> <br/> |<span data-ttu-id="1b82a-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="1b82a-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1b82a-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="1b82a-122">**Warning**</span></span> <br/> | <span data-ttu-id="1b82a-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="1b82a-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1b82a-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="1b82a-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1b82a-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="1b82a-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="1b82a-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="1b82a-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1b82a-127">– O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="1b82a-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="1b82a-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="1b82a-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1b82a-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="1b82a-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1b82a-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="1b82a-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1b82a-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="1b82a-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1b82a-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="1b82a-132">**Error**</span></span> <br/> | <span data-ttu-id="1b82a-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="1b82a-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1b82a-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="1b82a-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1b82a-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="1b82a-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1b82a-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="1b82a-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1b82a-137">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="1b82a-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="1b82a-138">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="1b82a-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1b82a-139">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="1b82a-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1b82a-140">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="1b82a-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1b82a-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1b82a-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1b82a-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1b82a-142">Child elements</span></span>

|<span data-ttu-id="1b82a-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b82a-143">**Element**</span></span>|<span data-ttu-id="1b82a-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b82a-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b82a-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1b82a-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1b82a-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b82a-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1b82a-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1b82a-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1b82a-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="1b82a-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1b82a-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1b82a-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1b82a-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="1b82a-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1b82a-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="1b82a-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1b82a-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1b82a-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1b82a-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="1b82a-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b82a-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1b82a-154">Parent elements</span></span>

|<span data-ttu-id="1b82a-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b82a-155">**Element**</span></span>|<span data-ttu-id="1b82a-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b82a-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b82a-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1b82a-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1b82a-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b82a-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b82a-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="1b82a-159">Remarks</span></span>

<span data-ttu-id="1b82a-160">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1b82a-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b82a-161">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1b82a-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b82a-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="1b82a-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b82a-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1b82a-163">Schema Name</span></span>  <br/> |<span data-ttu-id="1b82a-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1b82a-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b82a-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1b82a-165">Validation File</span></span>  <br/> |<span data-ttu-id="1b82a-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b82a-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b82a-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1b82a-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b82a-168">False</span><span class="sxs-lookup"><span data-stu-id="1b82a-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b82a-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="1b82a-169">See also</span></span>

- [<span data-ttu-id="1b82a-170">Operação RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="1b82a-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="1b82a-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1b82a-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

