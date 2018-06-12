---
title: MailTipsResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsResponseMessageType
api_type:
- schema
ms.assetid: 532cb9d9-1232-4e88-80aa-4cf163eb05da
description: O elemento MailTipsResponseMessageType representa as configurações de dicas de email.
ms.openlocfilehash: 76a1e33ae189b96a96a41d1bc7a8f79116761c4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824334"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="3a386-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="3a386-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="3a386-104">O elemento **MailTipsResponseMessageType** representa as configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="3a386-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="3a386-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3a386-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a386-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3a386-106">Attributes and elements</span></span>

<span data-ttu-id="3a386-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a386-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a386-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a386-108">Attributes</span></span>

|<span data-ttu-id="3a386-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="3a386-109">**Attribute**</span></span>|<span data-ttu-id="3a386-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a386-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a386-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3a386-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3a386-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a386-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="3a386-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="3a386-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3a386-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="3a386-114">-  Success</span></span>  <br/><span data-ttu-id="3a386-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="3a386-115">-  Warning</span></span>  <br/><span data-ttu-id="3a386-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="3a386-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3a386-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="3a386-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="3a386-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="3a386-118">**Value**</span></span>|<span data-ttu-id="3a386-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a386-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3a386-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="3a386-120">**Success**</span></span> <br/> |<span data-ttu-id="3a386-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="3a386-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3a386-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="3a386-122">**Warning**</span></span> <br/> | <span data-ttu-id="3a386-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="3a386-123">Describes a request that was not processed.</span></span> <span data-ttu-id="3a386-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="3a386-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3a386-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="3a386-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="3a386-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="3a386-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3a386-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="3a386-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3a386-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="3a386-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="3a386-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="3a386-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3a386-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="3a386-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="3a386-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="3a386-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="3a386-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="3a386-132">**Error**</span></span> <br/> | <span data-ttu-id="3a386-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="3a386-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3a386-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="3a386-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3a386-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3a386-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3a386-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="3a386-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="3a386-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="3a386-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="3a386-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="3a386-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="3a386-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="3a386-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3a386-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="3a386-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3a386-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="3a386-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3a386-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a386-142">Child elements</span></span>

|<span data-ttu-id="3a386-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a386-143">**Element**</span></span>|<span data-ttu-id="3a386-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a386-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a386-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="3a386-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3a386-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a386-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3a386-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3a386-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3a386-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a386-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3a386-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3a386-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3a386-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="3a386-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="3a386-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="3a386-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3a386-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3a386-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3a386-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="3a386-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3a386-154">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="3a386-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="3a386-155">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="3a386-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a386-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a386-156">Parent elements</span></span>

|<span data-ttu-id="3a386-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a386-157">**Element**</span></span>|<span data-ttu-id="3a386-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a386-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a386-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="3a386-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="3a386-160">Representa uma lista das mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="3a386-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a386-161">Text value</span><span class="sxs-lookup"><span data-stu-id="3a386-161">Text value</span></span>

<span data-ttu-id="3a386-162">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a386-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a386-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a386-163">Remarks</span></span>

<span data-ttu-id="3a386-164">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a386-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a386-165">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3a386-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a386-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a386-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a386-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a386-167">Schema Name</span></span>  <br/> |<span data-ttu-id="3a386-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3a386-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a386-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a386-169">Validation File</span></span>  <br/> |<span data-ttu-id="3a386-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a386-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a386-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3a386-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a386-172">False</span><span class="sxs-lookup"><span data-stu-id="3a386-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a386-173">Ver também</span><span class="sxs-lookup"><span data-stu-id="3a386-173">See also</span></span>

- [<span data-ttu-id="3a386-174">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3a386-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
