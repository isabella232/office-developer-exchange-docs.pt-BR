---
title: GetPhoneCallInformationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformationResponse
api_type:
- schema
ms.assetid: 17f79875-46ec-4289-b974-b3c35af429cd
description: O elemento de GetPhoneCallInformationResponse define uma resposta a uma única solicitação GetPhoneCallInformation.
ms.openlocfilehash: 5a03d63198cd00997b8975b18a5ae0eb5fca1af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752605"
---
# <a name="getphonecallinformationresponse"></a><span data-ttu-id="f57b7-103">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="f57b7-103">GetPhoneCallInformationResponse</span></span>

<span data-ttu-id="f57b7-104">O elemento de **GetPhoneCallInformationResponse** define uma resposta a uma única solicitação GetPhoneCallInformation.</span><span class="sxs-lookup"><span data-stu-id="f57b7-104">The **GetPhoneCallInformationResponse** element defines a response to a single GetPhoneCallInformation request.</span></span> 
  
```xml
<GetPhoneCallInformationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <PhoneCallInformation/>
</GetPhoneCallInformationResponse>
```

 <span data-ttu-id="f57b7-105">**GetPhoneCallInformationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f57b7-105">**GetPhoneCallInformationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f57b7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f57b7-106">Attributes and elements</span></span>

<span data-ttu-id="f57b7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f57b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f57b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f57b7-108">Attributes</span></span>

|<span data-ttu-id="f57b7-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="f57b7-109">**Attribute**</span></span>|<span data-ttu-id="f57b7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f57b7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f57b7-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f57b7-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f57b7-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="f57b7-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f57b7-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="f57b7-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="f57b7-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="f57b7-114">-  Success</span></span>  <br/><span data-ttu-id="f57b7-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="f57b7-115">-  Warning</span></span>  <br/><span data-ttu-id="f57b7-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="f57b7-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f57b7-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f57b7-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f57b7-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f57b7-118">**Value**</span></span>|<span data-ttu-id="f57b7-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f57b7-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f57b7-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="f57b7-120">**Success**</span></span> <br/> |<span data-ttu-id="f57b7-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="f57b7-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f57b7-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f57b7-122">**Warning**</span></span> <br/> | <span data-ttu-id="f57b7-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="f57b7-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f57b7-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="f57b7-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="f57b7-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="f57b7-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="f57b7-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="f57b7-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f57b7-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="f57b7-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="f57b7-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="f57b7-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f57b7-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="f57b7-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f57b7-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="f57b7-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f57b7-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="f57b7-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f57b7-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="f57b7-132">**Error**</span></span> <br/> | <span data-ttu-id="f57b7-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="f57b7-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f57b7-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="f57b7-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f57b7-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f57b7-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f57b7-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="f57b7-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f57b7-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="f57b7-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="f57b7-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="f57b7-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f57b7-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="f57b7-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f57b7-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="f57b7-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f57b7-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f57b7-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f57b7-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f57b7-142">Child elements</span></span>

|<span data-ttu-id="f57b7-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f57b7-143">**Element**</span></span>|<span data-ttu-id="f57b7-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f57b7-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f57b7-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f57b7-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f57b7-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="f57b7-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f57b7-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f57b7-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f57b7-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f57b7-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f57b7-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f57b7-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f57b7-150">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="f57b7-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f57b7-151">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="f57b7-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f57b7-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f57b7-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f57b7-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="f57b7-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f57b7-154">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="f57b7-154">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="f57b7-155">Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="f57b7-155">Specifies the state information for a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f57b7-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f57b7-156">Parent elements</span></span>

<span data-ttu-id="f57b7-157">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f57b7-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f57b7-158">Comentários</span><span class="sxs-lookup"><span data-stu-id="f57b7-158">Remarks</span></span>

<span data-ttu-id="f57b7-159">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f57b7-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f57b7-160">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f57b7-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f57b7-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="f57b7-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f57b7-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f57b7-162">Schema Name</span></span>  <br/> |<span data-ttu-id="f57b7-163">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f57b7-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f57b7-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f57b7-164">Validation File</span></span>  <br/> |<span data-ttu-id="f57b7-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f57b7-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f57b7-166">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f57b7-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="f57b7-167">False</span><span class="sxs-lookup"><span data-stu-id="f57b7-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f57b7-168">Ver também</span><span class="sxs-lookup"><span data-stu-id="f57b7-168">See also</span></span>

- [<span data-ttu-id="f57b7-169">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f57b7-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

