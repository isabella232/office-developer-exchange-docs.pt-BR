---
title: GetRoomsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomsResponse
api_type:
- schema
ms.assetid: a8c85f65-bb63-4e7a-b0ca-7c9a04560a58
description: O elemento GetRoomsResponse define uma resposta a uma solicitação de operação getrooms.
ms.openlocfilehash: 661e143a9edd30f12ab83fb0666e2832422e280a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458583"
---
# <a name="getroomsresponse"></a><span data-ttu-id="840d7-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="840d7-103">GetRoomsResponse</span></span>

<span data-ttu-id="840d7-104">O elemento **GetRoomsResponse** define uma resposta a uma solicitação de [operação getrooms](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="840d7-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="840d7-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="840d7-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="840d7-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="840d7-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="840d7-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="840d7-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="840d7-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="840d7-108">Attributes and elements</span></span>

<span data-ttu-id="840d7-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="840d7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="840d7-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="840d7-110">Attributes</span></span>

|<span data-ttu-id="840d7-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="840d7-111">**Attribute**</span></span>|<span data-ttu-id="840d7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="840d7-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="840d7-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="840d7-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="840d7-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="840d7-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="840d7-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="840d7-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="840d7-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="840d7-116">-  Success</span></span>  <br/><span data-ttu-id="840d7-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="840d7-117">-  Warning</span></span>  <br/><span data-ttu-id="840d7-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="840d7-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="840d7-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="840d7-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="840d7-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="840d7-120">**Value**</span></span>|<span data-ttu-id="840d7-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="840d7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="840d7-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="840d7-122">**Success**</span></span> <br/> |<span data-ttu-id="840d7-123">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="840d7-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="840d7-124">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="840d7-124">**Warning**</span></span> <br/> | <span data-ttu-id="840d7-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="840d7-125">Describes a request that was not processed.</span></span> <span data-ttu-id="840d7-126">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="840d7-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="840d7-127">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="840d7-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="840d7-128">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="840d7-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="840d7-129">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="840d7-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="840d7-130">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="840d7-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="840d7-131">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="840d7-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="840d7-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="840d7-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="840d7-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="840d7-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="840d7-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="840d7-134">**Error**</span></span> <br/> | <span data-ttu-id="840d7-135">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="840d7-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="840d7-136">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="840d7-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="840d7-137">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="840d7-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="840d7-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="840d7-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="840d7-139">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="840d7-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="840d7-140">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="840d7-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="840d7-141">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="840d7-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="840d7-142">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="840d7-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="840d7-143">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="840d7-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="840d7-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="840d7-144">Child elements</span></span>

|<span data-ttu-id="840d7-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="840d7-145">**Element**</span></span>|<span data-ttu-id="840d7-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="840d7-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="840d7-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="840d7-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="840d7-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="840d7-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="840d7-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="840d7-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="840d7-150">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="840d7-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="840d7-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="840d7-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="840d7-152">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="840d7-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="840d7-153">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="840d7-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="840d7-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="840d7-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="840d7-155">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="840d7-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="840d7-156">Quartos</span><span class="sxs-lookup"><span data-stu-id="840d7-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="840d7-157">Fornece uma lista de endereços de email e nomes de exibição que representam salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="840d7-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="840d7-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="840d7-158">Parent elements</span></span>

|<span data-ttu-id="840d7-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="840d7-159">**Element**</span></span>|<span data-ttu-id="840d7-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="840d7-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="840d7-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="840d7-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="840d7-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="840d7-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="840d7-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="840d7-163">Remarks</span></span>

<span data-ttu-id="840d7-164">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="840d7-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="840d7-165">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="840d7-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="840d7-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="840d7-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="840d7-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="840d7-167">Schema Name</span></span>  <br/> |<span data-ttu-id="840d7-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="840d7-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="840d7-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="840d7-169">Validation File</span></span>  <br/> |<span data-ttu-id="840d7-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="840d7-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="840d7-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="840d7-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="840d7-172">False</span><span class="sxs-lookup"><span data-stu-id="840d7-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="840d7-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="840d7-173">See also</span></span>

- [<span data-ttu-id="840d7-174">Operação getrooms</span><span class="sxs-lookup"><span data-stu-id="840d7-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="840d7-175">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="840d7-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

