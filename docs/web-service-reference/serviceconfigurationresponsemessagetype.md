---
title: ServiceConfigurationResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: O elemento ServiceConfigurationResponseMessageType contém definições de configuração de serviço.
ms.openlocfilehash: 4c84a49b2403343a1defd00696858489497d6214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44439102"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="71c95-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="71c95-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="71c95-104">O elemento **ServiceConfigurationResponseMessageType** contém definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="71c95-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="71c95-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="71c95-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71c95-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="71c95-106">Attributes and elements</span></span>

<span data-ttu-id="71c95-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="71c95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71c95-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="71c95-108">Attributes</span></span>

|<span data-ttu-id="71c95-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="71c95-109">**Attribute**</span></span>|<span data-ttu-id="71c95-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71c95-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71c95-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="71c95-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="71c95-112">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="71c95-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="71c95-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="71c95-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="71c95-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="71c95-114">-  Success</span></span>  <br/><span data-ttu-id="71c95-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="71c95-115">-  Warning</span></span>  <br/><span data-ttu-id="71c95-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="71c95-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="71c95-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="71c95-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="71c95-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="71c95-118">**Value**</span></span>|<span data-ttu-id="71c95-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71c95-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71c95-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="71c95-120">**Success**</span></span> <br/> |<span data-ttu-id="71c95-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="71c95-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="71c95-122">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="71c95-122">**Warning**</span></span> <br/> | <span data-ttu-id="71c95-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="71c95-123">Describes a request that was not processed.</span></span> <span data-ttu-id="71c95-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="71c95-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="71c95-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="71c95-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="71c95-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="71c95-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="71c95-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="71c95-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="71c95-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="71c95-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="71c95-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="71c95-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="71c95-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="71c95-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="71c95-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="71c95-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="71c95-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="71c95-132">**Error**</span></span> <br/> | <span data-ttu-id="71c95-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="71c95-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="71c95-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="71c95-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="71c95-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="71c95-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="71c95-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="71c95-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="71c95-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="71c95-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="71c95-138">-Um atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="71c95-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="71c95-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="71c95-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="71c95-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="71c95-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="71c95-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="71c95-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71c95-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="71c95-142">Child elements</span></span>

|<span data-ttu-id="71c95-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71c95-143">**Element**</span></span>|<span data-ttu-id="71c95-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71c95-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71c95-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="71c95-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="71c95-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="71c95-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="71c95-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="71c95-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="71c95-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="71c95-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="71c95-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="71c95-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="71c95-150">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="71c95-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="71c95-151">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="71c95-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="71c95-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="71c95-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71c95-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="71c95-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="71c95-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="71c95-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="71c95-155">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="71c95-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="71c95-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="71c95-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="71c95-157">Contém informações de configuração de serviço para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="71c95-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="71c95-158">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="71c95-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="71c95-159">Contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="71c95-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71c95-160">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="71c95-160">Parent elements</span></span>

|<span data-ttu-id="71c95-161">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71c95-161">**Element**</span></span>|<span data-ttu-id="71c95-162">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71c95-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71c95-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="71c95-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="71c95-164">Contém uma matriz de mensagens de resposta de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="71c95-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71c95-165">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="71c95-165">Text value</span></span>

<span data-ttu-id="71c95-166">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="71c95-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71c95-167">Comentários</span><span class="sxs-lookup"><span data-stu-id="71c95-167">Remarks</span></span>

<span data-ttu-id="71c95-168">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="71c95-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71c95-169">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="71c95-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71c95-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="71c95-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71c95-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="71c95-171">Schema Name</span></span>  <br/> |<span data-ttu-id="71c95-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="71c95-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71c95-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="71c95-173">Validation File</span></span>  <br/> |<span data-ttu-id="71c95-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="71c95-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71c95-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="71c95-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="71c95-176">False</span><span class="sxs-lookup"><span data-stu-id="71c95-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71c95-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="71c95-177">See also</span></span>

- [<span data-ttu-id="71c95-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="71c95-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

