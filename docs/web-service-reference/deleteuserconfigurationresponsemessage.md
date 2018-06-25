---
title: DeleteUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 543b1743-7e1c-4acb-93bd-34532e7fe79b
description: O elemento DeleteUserConfigurationResponseMessage contém o status e o resultado de uma única solicitação DeleteUserConfiguration.
ms.openlocfilehash: 3e07917688ad1f25f7ca3fa06d6db51cf9905503
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751768"
---
# <a name="deleteuserconfigurationresponsemessage"></a><span data-ttu-id="ded33-103">DeleteUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ded33-103">DeleteUserConfigurationResponseMessage</span></span>

<span data-ttu-id="ded33-104">O elemento **DeleteUserConfigurationResponseMessage** contém o status e o resultado de uma única solicitação **DeleteUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="ded33-104">The **DeleteUserConfigurationResponseMessage** element contains the status and result of a single **DeleteUserConfiguration** request.</span></span> 
  
```xml
<DeleteUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteUserConfigurationResponseMessage>
```

 <span data-ttu-id="ded33-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ded33-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ded33-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ded33-106">Attributes and elements</span></span>

<span data-ttu-id="ded33-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ded33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ded33-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ded33-108">Attributes</span></span>

|<span data-ttu-id="ded33-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="ded33-109">**Attribute**</span></span>|<span data-ttu-id="ded33-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ded33-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ded33-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ded33-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ded33-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="ded33-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="ded33-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="ded33-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="ded33-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="ded33-114">-  Success</span></span>  <br/><span data-ttu-id="ded33-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="ded33-115">-  Warning</span></span>  <br/><span data-ttu-id="ded33-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="ded33-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ded33-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ded33-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="ded33-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ded33-118">**Value**</span></span>|<span data-ttu-id="ded33-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ded33-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ded33-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="ded33-120">**Success**</span></span> <br/> |<span data-ttu-id="ded33-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="ded33-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ded33-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ded33-122">**Warning**</span></span> <br/> | <span data-ttu-id="ded33-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="ded33-123">Describes a request that was not processed.</span></span> <span data-ttu-id="ded33-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="ded33-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="ded33-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="ded33-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="ded33-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="ded33-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ded33-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="ded33-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ded33-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="ded33-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ded33-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="ded33-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ded33-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="ded33-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="ded33-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="ded33-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="ded33-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="ded33-132">**Error**</span></span> <br/> | <span data-ttu-id="ded33-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="ded33-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="ded33-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="ded33-134">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="ded33-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ded33-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ded33-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="ded33-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="ded33-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="ded33-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="ded33-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="ded33-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ded33-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="ded33-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ded33-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="ded33-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="ded33-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ded33-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ded33-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ded33-142">Child elements</span></span>

|<span data-ttu-id="ded33-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ded33-143">**Element**</span></span>|<span data-ttu-id="ded33-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ded33-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded33-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="ded33-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ded33-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="ded33-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ded33-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ded33-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ded33-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ded33-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ded33-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ded33-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ded33-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="ded33-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="ded33-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="ded33-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ded33-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ded33-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ded33-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="ded33-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ded33-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ded33-154">Parent elements</span></span>

|<span data-ttu-id="ded33-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ded33-155">**Element**</span></span>|<span data-ttu-id="ded33-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ded33-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded33-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ded33-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ded33-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ded33-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ded33-159">Text value</span><span class="sxs-lookup"><span data-stu-id="ded33-159">Text value</span></span>

<span data-ttu-id="ded33-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ded33-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ded33-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="ded33-161">Remarks</span></span>

<span data-ttu-id="ded33-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ded33-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ded33-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ded33-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ded33-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="ded33-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ded33-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ded33-165">Schema Name</span></span>  <br/> |<span data-ttu-id="ded33-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ded33-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ded33-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ded33-167">Validation File</span></span>  <br/> |<span data-ttu-id="ded33-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ded33-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ded33-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ded33-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="ded33-170">False</span><span class="sxs-lookup"><span data-stu-id="ded33-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ded33-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="ded33-171">See also</span></span>

- [<span data-ttu-id="ded33-172">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ded33-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

