---
title: PlayOnPhoneResponse (serviços Web do Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 578b70d1-dc9d-4bce-b859-0109b2d2bcec
description: O elemento PlayOnPhoneResponse especifica a resposta a uma solicitação para reproduzir uma mensagem de voz pelo telefone.
ms.openlocfilehash: 907864d7fe669aac99b2ff6d1c5eba71b9ddf79f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459620"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="99884-103">PlayOnPhoneResponse (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="99884-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="99884-104">O elemento **PlayOnPhoneResponse** especifica a resposta a uma solicitação para reproduzir uma mensagem de voz pelo telefone.</span><span class="sxs-lookup"><span data-stu-id="99884-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="99884-105">**PlayOnPhoneResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="99884-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99884-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="99884-106">Attributes and elements</span></span>

<span data-ttu-id="99884-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99884-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99884-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99884-108">Attributes</span></span>

|<span data-ttu-id="99884-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="99884-109">**Attribute**</span></span>|<span data-ttu-id="99884-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99884-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99884-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="99884-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="99884-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="99884-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="99884-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="99884-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="99884-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="99884-114">-  Success</span></span>  <br/><span data-ttu-id="99884-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="99884-115">-  Warning</span></span>  <br/><span data-ttu-id="99884-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="99884-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="99884-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="99884-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="99884-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="99884-118">**Value**</span></span>|<span data-ttu-id="99884-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99884-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99884-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="99884-120">**Success**</span></span> <br/> |<span data-ttu-id="99884-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="99884-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="99884-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="99884-122">**Warning**</span></span> <br/> | <span data-ttu-id="99884-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="99884-123">Describes a request that was not processed.</span></span> <span data-ttu-id="99884-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="99884-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="99884-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="99884-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="99884-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="99884-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="99884-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="99884-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="99884-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="99884-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="99884-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="99884-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="99884-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="99884-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="99884-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="99884-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="99884-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="99884-132">**Error**</span></span> <br/> | <span data-ttu-id="99884-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="99884-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="99884-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="99884-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="99884-135">-Atributos ou elementos inválidos.</span><span class="sxs-lookup"><span data-stu-id="99884-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="99884-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="99884-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="99884-137">-Uma marca desconhecida.</span><span class="sxs-lookup"><span data-stu-id="99884-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="99884-138">-Um atributo ou elemento que não é válido no contexto.</span><span class="sxs-lookup"><span data-stu-id="99884-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="99884-139">– Uma tentativa de acesso não autorizado por qualquer cliente.</span><span class="sxs-lookup"><span data-stu-id="99884-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="99884-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="99884-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="99884-141">As informações sobre o erro podem ser encontradas nos tópicos do elemento [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="99884-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="99884-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99884-142">Child elements</span></span>

|<span data-ttu-id="99884-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="99884-143">**Element**</span></span>|<span data-ttu-id="99884-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99884-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99884-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="99884-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="99884-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="99884-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="99884-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="99884-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="99884-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="99884-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="99884-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="99884-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="99884-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="99884-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="99884-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="99884-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="99884-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="99884-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="99884-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="99884-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="99884-154">Chamada de chamada</span><span class="sxs-lookup"><span data-stu-id="99884-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="99884-155">Especifica o identificador de chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="99884-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99884-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99884-156">Parent elements</span></span>

<span data-ttu-id="99884-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99884-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99884-158">Comentários</span><span class="sxs-lookup"><span data-stu-id="99884-158">Remarks</span></span>

<span data-ttu-id="99884-159">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99884-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99884-160">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="99884-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99884-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="99884-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99884-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99884-162">Schema Name</span></span>  <br/> |<span data-ttu-id="99884-163">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="99884-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99884-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99884-164">Validation File</span></span>  <br/> |<span data-ttu-id="99884-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="99884-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99884-166">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="99884-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="99884-167">False</span><span class="sxs-lookup"><span data-stu-id="99884-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99884-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="99884-168">See also</span></span>

- [<span data-ttu-id="99884-169">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="99884-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

