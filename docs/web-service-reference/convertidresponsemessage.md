---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: O elemento ConvertIdResponseMessage contém o status e o resultado de uma solicitação de operação ConvertId.
ms.openlocfilehash: 6668c0b3254191ca628413bae5ff957c3cb95b5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751547"
---
# <a name="convertidresponsemessage"></a><span data-ttu-id="50b8d-103">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="50b8d-103">ConvertIdResponseMessage</span></span>

<span data-ttu-id="50b8d-104">O elemento **ConvertIdResponseMessage** contém o status e o resultado de uma solicitação de [operação ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50b8d-104">The **ConvertIdResponseMessage** element contains the status and result of a [ConvertId operation](convertid-operation.md) request.</span></span> 
  
- [<span data-ttu-id="50b8d-105">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="50b8d-105">ConvertIdResponse</span></span>](convertidresponse.md) 
- [<span data-ttu-id="50b8d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50b8d-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="50b8d-107">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="50b8d-107">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 <span data-ttu-id="50b8d-108">**ConvertIdResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="50b8d-108">**ConvertIdResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50b8d-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="50b8d-109">Attributes and elements</span></span>

<span data-ttu-id="50b8d-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="50b8d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50b8d-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="50b8d-111">Attributes</span></span>

|<span data-ttu-id="50b8d-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="50b8d-112">**Attribute**</span></span>|<span data-ttu-id="50b8d-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50b8d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50b8d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="50b8d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="50b8d-115">Descreve o status de uma resposta de [operação ConvertId](convertid-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="50b8d-115">Describes the status of a [ConvertId operation](convertid-operation.md) response.</span></span><br/><br/><span data-ttu-id="50b8d-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="50b8d-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="50b8d-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="50b8d-117">- Success</span></span>  <br/><span data-ttu-id="50b8d-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="50b8d-118">-  Warning</span></span>  <br/><span data-ttu-id="50b8d-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="50b8d-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="50b8d-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="50b8d-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="50b8d-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="50b8d-121">**Value**</span></span>|<span data-ttu-id="50b8d-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50b8d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50b8d-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="50b8d-123">**Success**</span></span> <br/> |<span data-ttu-id="50b8d-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="50b8d-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="50b8d-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="50b8d-125">**Warning**</span></span> <br/> | <span data-ttu-id="50b8d-126">Descreve uma solicitação que ainda não foi totalmente processada ou para os quais um resultado acidentais ocorreu.</span><span class="sxs-lookup"><span data-stu-id="50b8d-126">Describes a request that was not fully processed or for which an unintended result occurred.</span></span>  <br/> |
|<span data-ttu-id="50b8d-127">**Erro**</span><span class="sxs-lookup"><span data-stu-id="50b8d-127">**Error**</span></span> <br/> | <span data-ttu-id="50b8d-128">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="50b8d-128">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="50b8d-129">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="50b8d-129">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="50b8d-130">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="50b8d-130">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="50b8d-131">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="50b8d-131">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="50b8d-132">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="50b8d-132">-  An unknown tag</span></span>  <br/><span data-ttu-id="50b8d-133">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="50b8d-133">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="50b8d-134">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="50b8d-134">- An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="50b8d-135">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="50b8d-135">-  A server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="50b8d-136">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="50b8d-136">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="50b8d-137">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="50b8d-137">Child elements</span></span>

|<span data-ttu-id="50b8d-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50b8d-138">**Element**</span></span>|<span data-ttu-id="50b8d-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50b8d-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50b8d-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="50b8d-140">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="50b8d-141">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="50b8d-141">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="50b8d-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50b8d-142">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="50b8d-143">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="50b8d-143">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="50b8d-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="50b8d-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="50b8d-145">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="50b8d-145">Currently unused and reserved for future use.</span></span> <span data-ttu-id="50b8d-146">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="50b8d-146">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="50b8d-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="50b8d-147">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="50b8d-148">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="50b8d-148">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="50b8d-149">AlternateId</span><span class="sxs-lookup"><span data-stu-id="50b8d-149">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="50b8d-150">Descreve um identificador convertido na resposta.</span><span class="sxs-lookup"><span data-stu-id="50b8d-150">Describes a converted identifier in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50b8d-151">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="50b8d-151">Parent elements</span></span>

|<span data-ttu-id="50b8d-152">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50b8d-152">**Element**</span></span>|<span data-ttu-id="50b8d-153">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50b8d-153">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50b8d-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50b8d-154">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="50b8d-155">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="50b8d-155">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50b8d-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="50b8d-156">Remarks</span></span>

<span data-ttu-id="50b8d-157">Uma mensagem de resposta por identificador convertido será retornada.</span><span class="sxs-lookup"><span data-stu-id="50b8d-157">One response message per converted identifier is returned.</span></span> <span data-ttu-id="50b8d-158">O elemento [AlternateId](alternateid.md) serão ausente da resposta se um código de resposta de erro é retornado,</span><span class="sxs-lookup"><span data-stu-id="50b8d-158">The [AlternateId](alternateid.md) element will be missing from the response if an error response code is returned,</span></span> 
  
<span data-ttu-id="50b8d-159">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="50b8d-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50b8d-160">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="50b8d-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50b8d-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="50b8d-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50b8d-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="50b8d-162">Schema Name</span></span>  <br/> |<span data-ttu-id="50b8d-163">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="50b8d-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50b8d-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="50b8d-164">Validation File</span></span>  <br/> |<span data-ttu-id="50b8d-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="50b8d-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50b8d-166">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="50b8d-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="50b8d-167">False</span><span class="sxs-lookup"><span data-stu-id="50b8d-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50b8d-168">Ver também</span><span class="sxs-lookup"><span data-stu-id="50b8d-168">See also</span></span>

- [<span data-ttu-id="50b8d-169">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="50b8d-169">ConvertId operation</span></span>](convertid-operation.md)
- [<span data-ttu-id="50b8d-170">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50b8d-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

