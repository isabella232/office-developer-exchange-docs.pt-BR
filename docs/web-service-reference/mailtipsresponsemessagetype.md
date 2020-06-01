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
description: O elemento MailTipsResponseMessageType representa configurações de dicas de email.
ms.openlocfilehash: 5244f26ef927a817a9087c299fd1124acb828aa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454033"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="bc861-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="bc861-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="bc861-104">O elemento **MailTipsResponseMessageType** representa configurações de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="bc861-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="bc861-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bc861-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc861-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bc861-106">Attributes and elements</span></span>

<span data-ttu-id="bc861-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bc861-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc861-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bc861-108">Attributes</span></span>

|<span data-ttu-id="bc861-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="bc861-109">**Attribute**</span></span>|<span data-ttu-id="bc861-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc861-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc861-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bc861-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bc861-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc861-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="bc861-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="bc861-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="bc861-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="bc861-114">-  Success</span></span>  <br/><span data-ttu-id="bc861-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="bc861-115">-  Warning</span></span>  <br/><span data-ttu-id="bc861-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="bc861-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bc861-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bc861-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="bc861-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="bc861-118">**Value**</span></span>|<span data-ttu-id="bc861-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc861-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc861-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="bc861-120">**Success**</span></span> <br/> |<span data-ttu-id="bc861-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="bc861-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bc861-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="bc861-122">**Warning**</span></span> <br/> | <span data-ttu-id="bc861-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="bc861-123">Describes a request that was not processed.</span></span> <span data-ttu-id="bc861-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="bc861-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="bc861-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="bc861-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="bc861-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="bc861-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bc861-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="bc861-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bc861-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="bc861-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bc861-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="bc861-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bc861-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="bc861-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="bc861-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="bc861-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bc861-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="bc861-132">**Error**</span></span> <br/> | <span data-ttu-id="bc861-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="bc861-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bc861-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="bc861-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bc861-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="bc861-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bc861-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="bc861-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="bc861-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="bc861-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="bc861-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="bc861-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="bc861-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="bc861-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bc861-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="bc861-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="bc861-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bc861-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc861-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bc861-142">Child elements</span></span>

|<span data-ttu-id="bc861-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bc861-143">**Element**</span></span>|<span data-ttu-id="bc861-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc861-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc861-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="bc861-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bc861-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc861-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bc861-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bc861-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bc861-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="bc861-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bc861-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bc861-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bc861-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="bc861-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bc861-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="bc861-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bc861-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bc861-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bc861-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="bc861-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bc861-154">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="bc861-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="bc861-155">Representa valores de vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="bc861-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc861-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bc861-156">Parent elements</span></span>

|<span data-ttu-id="bc861-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bc861-157">**Element**</span></span>|<span data-ttu-id="bc861-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc861-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc861-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="bc861-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="bc861-160">Representa uma lista de mensagens de resposta de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="bc861-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc861-161">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bc861-161">Text value</span></span>

<span data-ttu-id="bc861-162">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bc861-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc861-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="bc861-163">Remarks</span></span>

<span data-ttu-id="bc861-164">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc861-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc861-165">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bc861-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc861-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="bc861-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc861-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bc861-167">Schema Name</span></span>  <br/> |<span data-ttu-id="bc861-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="bc861-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc861-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bc861-169">Validation File</span></span>  <br/> |<span data-ttu-id="bc861-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bc861-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc861-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bc861-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc861-172">False</span><span class="sxs-lookup"><span data-stu-id="bc861-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc861-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc861-173">See also</span></span>

- [<span data-ttu-id="bc861-174">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bc861-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

