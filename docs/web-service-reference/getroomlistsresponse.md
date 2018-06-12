---
title: GetRoomListsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomListsResponse
api_type:
- schema
ms.assetid: 8c736f68-1026-496a-b12f-c169c078abd0
description: O elemento de GetRoomListsResponse define a resposta de uma solicitação de operação GetRoomLists.
ms.openlocfilehash: 8231435f7dc348a070852f57d6152550326b5df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752623"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="add0b-103">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="add0b-103">GetRoomListsResponse</span></span>

<span data-ttu-id="add0b-104">O elemento de **GetRoomListsResponse** define a resposta de uma solicitação de [operação GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="add0b-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="add0b-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="add0b-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="add0b-106">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="add0b-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="add0b-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="add0b-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="add0b-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="add0b-108">Attributes and elements</span></span>

<span data-ttu-id="add0b-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="add0b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="add0b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="add0b-110">Attributes</span></span>

|<span data-ttu-id="add0b-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="add0b-111">**Attribute**</span></span>|<span data-ttu-id="add0b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="add0b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="add0b-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="add0b-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="add0b-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="add0b-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="add0b-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="add0b-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="add0b-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="add0b-116">-  Success</span></span>  <br/><span data-ttu-id="add0b-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="add0b-117">-  Warning</span></span>  <br/><span data-ttu-id="add0b-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="add0b-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="add0b-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="add0b-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="add0b-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="add0b-120">**Value**</span></span>|<span data-ttu-id="add0b-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="add0b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="add0b-122">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="add0b-122">**Success**</span></span> <br/> |<span data-ttu-id="add0b-123">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="add0b-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="add0b-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="add0b-124">**Warning**</span></span> <br/> | <span data-ttu-id="add0b-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="add0b-125">Describes a request that was not processed.</span></span> <span data-ttu-id="add0b-126">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="add0b-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="add0b-127">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="add0b-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="add0b-128">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="add0b-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="add0b-129">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="add0b-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="add0b-130">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="add0b-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="add0b-131">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="add0b-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="add0b-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="add0b-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="add0b-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="add0b-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="add0b-134">**Erro**</span><span class="sxs-lookup"><span data-stu-id="add0b-134">**Error**</span></span> <br/> | <span data-ttu-id="add0b-135">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="add0b-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="add0b-136">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="add0b-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="add0b-137">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="add0b-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="add0b-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="add0b-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="add0b-139">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="add0b-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="add0b-140">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="add0b-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="add0b-141">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="add0b-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="add0b-142">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="add0b-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="add0b-143">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="add0b-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="add0b-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="add0b-144">Child elements</span></span>

|<span data-ttu-id="add0b-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="add0b-145">**Element**</span></span>|<span data-ttu-id="add0b-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="add0b-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="add0b-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="add0b-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="add0b-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="add0b-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="add0b-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="add0b-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="add0b-150">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="add0b-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="add0b-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="add0b-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="add0b-152">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="add0b-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="add0b-153">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="add0b-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="add0b-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="add0b-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="add0b-155">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="add0b-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="add0b-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="add0b-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="add0b-157">Fornece uma lista de endereços de email e nomes para exibição que representam listas de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="add0b-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="add0b-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="add0b-158">Parent elements</span></span>

|<span data-ttu-id="add0b-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="add0b-159">**Element**</span></span>|<span data-ttu-id="add0b-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="add0b-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="add0b-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="add0b-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="add0b-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="add0b-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="add0b-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="add0b-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="add0b-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="add0b-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="add0b-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="add0b-165">Schema Name</span></span>  <br/> |<span data-ttu-id="add0b-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="add0b-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="add0b-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="add0b-167">Validation File</span></span>  <br/> |<span data-ttu-id="add0b-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="add0b-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="add0b-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="add0b-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="add0b-170">False</span><span class="sxs-lookup"><span data-stu-id="add0b-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="add0b-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="add0b-171">See also</span></span>

- [<span data-ttu-id="add0b-172">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="add0b-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="add0b-173">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="add0b-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

