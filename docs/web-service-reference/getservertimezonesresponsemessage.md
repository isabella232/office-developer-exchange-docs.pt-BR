---
title: GetServerTimeZonesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponseMessage
api_type:
- schema
ms.assetid: eb2592b2-144f-4c33-8df7-8e70dce7ab55
description: O elemento GetServerTimeZonesResponseMessage contém o status e o resultado de uma única solicitação de operação de GetServerTimeZones.
ms.openlocfilehash: de032c961f6fffa5b4f0607a17fe48630510fda9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460915"
---
# <a name="getservertimezonesresponsemessage"></a><span data-ttu-id="70ea1-103">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="70ea1-103">GetServerTimeZonesResponseMessage</span></span>

<span data-ttu-id="70ea1-104">O elemento **GetServerTimeZonesResponseMessage** contém o status e o resultado de uma única solicitação de [operação de GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="70ea1-104">The **GetServerTimeZonesResponseMessage** element contains the status and result of a single [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <TimeZoneDefinitions/>
</GetServerTimeZonesResponseMessage>
```

 <span data-ttu-id="70ea1-105">**GetServerTimeZonesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="70ea1-105">**GetServerTimeZonesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70ea1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="70ea1-106">Attributes and elements</span></span>

<span data-ttu-id="70ea1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70ea1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70ea1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="70ea1-108">Attributes</span></span>

|<span data-ttu-id="70ea1-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="70ea1-109">**Attribute**</span></span>|<span data-ttu-id="70ea1-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ea1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70ea1-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="70ea1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="70ea1-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="70ea1-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="70ea1-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="70ea1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="70ea1-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="70ea1-114">-  Success</span></span>  <br/><span data-ttu-id="70ea1-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="70ea1-115">-  Warning</span></span>  <br/><span data-ttu-id="70ea1-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="70ea1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="70ea1-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="70ea1-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="70ea1-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="70ea1-118">**Value**</span></span>|<span data-ttu-id="70ea1-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ea1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70ea1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="70ea1-120">**Success**</span></span> <br/> |<span data-ttu-id="70ea1-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="70ea1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="70ea1-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="70ea1-122">**Warning**</span></span> <br/> | <span data-ttu-id="70ea1-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="70ea1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="70ea1-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="70ea1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="70ea1-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="70ea1-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="70ea1-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="70ea1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="70ea1-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="70ea1-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="70ea1-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="70ea1-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="70ea1-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="70ea1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="70ea1-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="70ea1-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="70ea1-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="70ea1-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="70ea1-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="70ea1-132">**Error**</span></span> <br/> | <span data-ttu-id="70ea1-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="70ea1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="70ea1-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="70ea1-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="70ea1-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="70ea1-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="70ea1-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="70ea1-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="70ea1-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="70ea1-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="70ea1-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="70ea1-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="70ea1-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="70ea1-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="70ea1-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="70ea1-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="70ea1-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="70ea1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70ea1-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70ea1-142">Child elements</span></span>

|<span data-ttu-id="70ea1-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70ea1-143">**Element**</span></span>|<span data-ttu-id="70ea1-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ea1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70ea1-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="70ea1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="70ea1-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="70ea1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="70ea1-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="70ea1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="70ea1-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="70ea1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="70ea1-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="70ea1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="70ea1-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="70ea1-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="70ea1-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="70ea1-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="70ea1-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="70ea1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="70ea1-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="70ea1-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="70ea1-154">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="70ea1-154">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="70ea1-155">Contém uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="70ea1-155">Contains an array of time zone definitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70ea1-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70ea1-156">Parent elements</span></span>

|<span data-ttu-id="70ea1-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70ea1-157">**Element**</span></span>|<span data-ttu-id="70ea1-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ea1-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70ea1-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="70ea1-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="70ea1-160">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="70ea1-160">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70ea1-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="70ea1-161">Remarks</span></span>

<span data-ttu-id="70ea1-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70ea1-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70ea1-163">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="70ea1-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70ea1-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="70ea1-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70ea1-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70ea1-165">Schema Name</span></span>  <br/> |<span data-ttu-id="70ea1-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="70ea1-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70ea1-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70ea1-167">Validation File</span></span>  <br/> |<span data-ttu-id="70ea1-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70ea1-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70ea1-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="70ea1-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="70ea1-170">False</span><span class="sxs-lookup"><span data-stu-id="70ea1-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70ea1-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="70ea1-171">See also</span></span>

- [<span data-ttu-id="70ea1-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="70ea1-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

