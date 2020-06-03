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
description: O elemento GetRoomListsResponse define a resposta de uma solicitação de operação GetRoomLists.
ms.openlocfilehash: b6d7c2baa2861309d72bcbf880eaed2ad0989175
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462940"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="b70f8-103">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="b70f8-103">GetRoomListsResponse</span></span>

<span data-ttu-id="b70f8-104">O elemento **GetRoomListsResponse** define a resposta de uma solicitação de [operação GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b70f8-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b70f8-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b70f8-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b70f8-106">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="b70f8-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="b70f8-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b70f8-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b70f8-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b70f8-108">Attributes and elements</span></span>

<span data-ttu-id="b70f8-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b70f8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b70f8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b70f8-110">Attributes</span></span>

|<span data-ttu-id="b70f8-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b70f8-111">**Attribute**</span></span>|<span data-ttu-id="b70f8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b70f8-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b70f8-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b70f8-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b70f8-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b70f8-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b70f8-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="b70f8-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b70f8-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="b70f8-116">-  Success</span></span>  <br/><span data-ttu-id="b70f8-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="b70f8-117">-  Warning</span></span>  <br/><span data-ttu-id="b70f8-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="b70f8-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b70f8-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b70f8-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="b70f8-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b70f8-120">**Value**</span></span>|<span data-ttu-id="b70f8-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b70f8-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b70f8-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="b70f8-122">**Success**</span></span> <br/> |<span data-ttu-id="b70f8-123">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="b70f8-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b70f8-124">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="b70f8-124">**Warning**</span></span> <br/> | <span data-ttu-id="b70f8-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="b70f8-125">Describes a request that was not processed.</span></span> <span data-ttu-id="b70f8-126">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="b70f8-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b70f8-127">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="b70f8-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b70f8-128">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="b70f8-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b70f8-129">– O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="b70f8-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="b70f8-130">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="b70f8-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b70f8-131">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="b70f8-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b70f8-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="b70f8-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="b70f8-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="b70f8-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b70f8-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="b70f8-134">**Error**</span></span> <br/> | <span data-ttu-id="b70f8-135">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="b70f8-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b70f8-136">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="b70f8-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b70f8-137">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="b70f8-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b70f8-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="b70f8-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b70f8-139">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="b70f8-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="b70f8-140">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="b70f8-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b70f8-141">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="b70f8-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b70f8-142">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="b70f8-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b70f8-143">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b70f8-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="b70f8-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b70f8-144">Child elements</span></span>

|<span data-ttu-id="b70f8-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b70f8-145">**Element**</span></span>|<span data-ttu-id="b70f8-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b70f8-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b70f8-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="b70f8-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b70f8-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b70f8-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b70f8-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b70f8-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b70f8-150">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="b70f8-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b70f8-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b70f8-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b70f8-152">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="b70f8-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b70f8-153">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="b70f8-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b70f8-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b70f8-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b70f8-155">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="b70f8-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b70f8-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="b70f8-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="b70f8-157">Fornece uma lista de endereços de email e nomes de exibição que representam listas de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="b70f8-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b70f8-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b70f8-158">Parent elements</span></span>

|<span data-ttu-id="b70f8-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b70f8-159">**Element**</span></span>|<span data-ttu-id="b70f8-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b70f8-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b70f8-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b70f8-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b70f8-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b70f8-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="b70f8-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b70f8-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b70f8-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="b70f8-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b70f8-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b70f8-165">Schema Name</span></span>  <br/> |<span data-ttu-id="b70f8-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b70f8-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b70f8-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b70f8-167">Validation File</span></span>  <br/> |<span data-ttu-id="b70f8-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b70f8-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b70f8-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b70f8-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="b70f8-170">False</span><span class="sxs-lookup"><span data-stu-id="b70f8-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b70f8-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="b70f8-171">See also</span></span>

- [<span data-ttu-id="b70f8-172">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="b70f8-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="b70f8-173">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b70f8-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

