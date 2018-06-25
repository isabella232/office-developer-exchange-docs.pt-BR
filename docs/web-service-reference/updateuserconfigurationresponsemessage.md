---
title: UpdateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 27728e57-5a9b-4314-ad64-df7869098f62
description: O elemento UpdateUserConfigurationResponseMessage contém o status e o resultado de uma única solicitação de operação UpdateUserConfiguration.
ms.openlocfilehash: db26bb4bc821ac9a09c350009ab8132466e759bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837947"
---
# <a name="updateuserconfigurationresponsemessage"></a><span data-ttu-id="ef708-103">UpdateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef708-103">UpdateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="ef708-104">O elemento **UpdateUserConfigurationResponseMessage** contém o status e o resultado de uma única solicitação de operação UpdateUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef708-104">The **UpdateUserConfigurationResponseMessage** element contains the status and result of a single UpdateUserConfiguration operation request.</span></span> 
  
```xml
<UpdateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateUserConfigurationResponseMessage>
```

 <span data-ttu-id="ef708-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ef708-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef708-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ef708-106">Attributes and elements</span></span>

<span data-ttu-id="ef708-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef708-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef708-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef708-108">Attributes</span></span>

|<span data-ttu-id="ef708-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="ef708-109">**Attribute**</span></span>|<span data-ttu-id="ef708-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef708-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef708-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ef708-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ef708-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef708-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="ef708-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="ef708-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="ef708-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="ef708-114">-  Success</span></span>  <br/><span data-ttu-id="ef708-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="ef708-115">-  Warning</span></span>  <br/><span data-ttu-id="ef708-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="ef708-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ef708-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ef708-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="ef708-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ef708-118">**Value**</span></span>|<span data-ttu-id="ef708-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef708-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef708-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="ef708-120">**Success**</span></span> <br/> |<span data-ttu-id="ef708-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="ef708-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ef708-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ef708-122">**Warning**</span></span> <br/> | <span data-ttu-id="ef708-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="ef708-123">Describes a request that was not processed.</span></span> <span data-ttu-id="ef708-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="ef708-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ef708-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="ef708-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ef708-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="ef708-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ef708-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="ef708-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="ef708-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="ef708-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ef708-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="ef708-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ef708-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="ef708-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="ef708-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="ef708-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="ef708-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="ef708-132">**Error**</span></span> <br/> | <span data-ttu-id="ef708-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="ef708-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ef708-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="ef708-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ef708-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ef708-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ef708-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="ef708-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ef708-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="ef708-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="ef708-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="ef708-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="ef708-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="ef708-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ef708-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="ef708-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ef708-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ef708-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef708-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef708-142">Child elements</span></span>

|<span data-ttu-id="ef708-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef708-143">**Element**</span></span>|<span data-ttu-id="ef708-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef708-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef708-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="ef708-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ef708-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef708-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ef708-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ef708-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ef708-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef708-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ef708-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ef708-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ef708-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="ef708-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="ef708-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="ef708-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ef708-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ef708-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ef708-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="ef708-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef708-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef708-154">Parent elements</span></span>

|<span data-ttu-id="ef708-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef708-155">**Element**</span></span>|<span data-ttu-id="ef708-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef708-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef708-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef708-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ef708-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef708-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef708-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef708-159">Remarks</span></span>

<span data-ttu-id="ef708-160">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ef708-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef708-161">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ef708-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef708-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef708-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef708-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef708-163">Schema Name</span></span>  <br/> |<span data-ttu-id="ef708-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ef708-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ef708-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef708-165">Validation File</span></span>  <br/> |<span data-ttu-id="ef708-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ef708-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef708-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef708-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef708-168">False</span><span class="sxs-lookup"><span data-stu-id="ef708-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef708-169">Ver também</span><span class="sxs-lookup"><span data-stu-id="ef708-169">See also</span></span>

- [<span data-ttu-id="ef708-170">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ef708-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

