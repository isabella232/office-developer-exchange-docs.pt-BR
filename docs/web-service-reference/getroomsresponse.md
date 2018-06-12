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
description: O elemento de GetRoomsResponse define uma resposta a uma solicitação de operação GetRooms.
ms.openlocfilehash: 7399ab910a99b39757eb752b11a4771ba81be46a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752617"
---
# <a name="getroomsresponse"></a><span data-ttu-id="5795b-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="5795b-103">GetRoomsResponse</span></span>

<span data-ttu-id="5795b-104">O elemento de **GetRoomsResponse** define uma resposta a uma solicitação de [operação GetRooms](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5795b-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5795b-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5795b-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="5795b-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="5795b-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="5795b-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5795b-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5795b-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5795b-108">Attributes and elements</span></span>

<span data-ttu-id="5795b-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5795b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5795b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="5795b-110">Attributes</span></span>

|<span data-ttu-id="5795b-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5795b-111">**Attribute**</span></span>|<span data-ttu-id="5795b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5795b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5795b-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5795b-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5795b-114">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5795b-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="5795b-115">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="5795b-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="5795b-116">-Êxito</span><span class="sxs-lookup"><span data-stu-id="5795b-116">-  Success</span></span>  <br/><span data-ttu-id="5795b-117">-Aviso</span><span class="sxs-lookup"><span data-stu-id="5795b-117">-  Warning</span></span>  <br/><span data-ttu-id="5795b-118">-Erro</span><span class="sxs-lookup"><span data-stu-id="5795b-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5795b-119">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5795b-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="5795b-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5795b-120">**Value**</span></span>|<span data-ttu-id="5795b-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5795b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5795b-122">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="5795b-122">**Success**</span></span> <br/> |<span data-ttu-id="5795b-123">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="5795b-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5795b-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5795b-124">**Warning**</span></span> <br/> | <span data-ttu-id="5795b-125">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="5795b-125">Describes a request that was not processed.</span></span> <span data-ttu-id="5795b-126">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="5795b-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5795b-127">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="5795b-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="5795b-128">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="5795b-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5795b-129">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="5795b-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5795b-130">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="5795b-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="5795b-131">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="5795b-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5795b-132">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="5795b-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="5795b-133">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="5795b-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="5795b-134">**Erro**</span><span class="sxs-lookup"><span data-stu-id="5795b-134">**Error**</span></span> <br/> | <span data-ttu-id="5795b-135">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="5795b-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5795b-136">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="5795b-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5795b-137">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5795b-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5795b-138">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="5795b-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="5795b-139">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="5795b-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="5795b-140">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="5795b-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="5795b-141">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="5795b-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5795b-142">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="5795b-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5795b-143">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5795b-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5795b-144">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5795b-144">Child elements</span></span>

|<span data-ttu-id="5795b-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5795b-145">**Element**</span></span>|<span data-ttu-id="5795b-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5795b-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5795b-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="5795b-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5795b-148">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5795b-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5795b-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5795b-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5795b-150">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5795b-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5795b-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5795b-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5795b-152">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5795b-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="5795b-153">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="5795b-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5795b-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5795b-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5795b-155">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="5795b-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5795b-156">Salas</span><span class="sxs-lookup"><span data-stu-id="5795b-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="5795b-157">Fornece uma lista de endereços de email e nomes para exibição que representam as salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="5795b-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5795b-158">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5795b-158">Parent elements</span></span>

|<span data-ttu-id="5795b-159">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5795b-159">**Element**</span></span>|<span data-ttu-id="5795b-160">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5795b-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5795b-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5795b-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5795b-162">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5795b-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5795b-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="5795b-163">Remarks</span></span>

<span data-ttu-id="5795b-164">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5795b-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5795b-165">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5795b-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5795b-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="5795b-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5795b-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5795b-167">Schema Name</span></span>  <br/> |<span data-ttu-id="5795b-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5795b-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5795b-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5795b-169">Validation File</span></span>  <br/> |<span data-ttu-id="5795b-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5795b-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5795b-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5795b-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="5795b-172">False</span><span class="sxs-lookup"><span data-stu-id="5795b-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5795b-173">Ver também</span><span class="sxs-lookup"><span data-stu-id="5795b-173">See also</span></span>

- [<span data-ttu-id="5795b-174">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="5795b-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="5795b-175">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5795b-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

