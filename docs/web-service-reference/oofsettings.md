---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: O elemento OofSettings contém as configurações de fora do escritório (OOF).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824649"
---
# <a name="oofsettings"></a><span data-ttu-id="3a5fc-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3a5fc-103">OofSettings</span></span>

<span data-ttu-id="3a5fc-104">O elemento **OofSettings** contém as configurações de fora do escritório (OOF).</span><span class="sxs-lookup"><span data-stu-id="3a5fc-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="3a5fc-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3a5fc-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="3a5fc-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3a5fc-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="3a5fc-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="3a5fc-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a5fc-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3a5fc-108">Attributes and elements</span></span>

<span data-ttu-id="3a5fc-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a5fc-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a5fc-110">Attributes</span></span>

<span data-ttu-id="3a5fc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a5fc-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a5fc-112">Child elements</span></span>

|<span data-ttu-id="3a5fc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a5fc-113">**Element**</span></span>|<span data-ttu-id="3a5fc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a5fc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5fc-115">OofState</span><span class="sxs-lookup"><span data-stu-id="3a5fc-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="3a5fc-116">Contém o estado de ausência temporária do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="3a5fc-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="3a5fc-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="3a5fc-118">Contém um valor que determina a quem as mensagens de ausência temporária externas são enviadas.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="3a5fc-119">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="3a5fc-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="3a5fc-120">Contém a duração em que o status de ausência temporária está ativado se o elemento [OofState](oofstate.md) for definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="3a5fc-121">Se o elemento [OofState](oofstate.md) for definido como **habilitado** ou **desabilitado**, o valor deste elemento será ignorado.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="3a5fc-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="3a5fc-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="3a5fc-123">Contém a resposta de ausência temporária enviada para outros usuários no domínio do usuário ou o domínio confiável.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="3a5fc-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="3a5fc-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="3a5fc-125">Contém a resposta de ausência temporária enviada para endereços fora do domínio ou os domínios confiáveis do destinatário.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a5fc-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a5fc-126">Parent elements</span></span>

|<span data-ttu-id="3a5fc-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a5fc-127">**Element**</span></span>|<span data-ttu-id="3a5fc-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a5fc-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a5fc-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3a5fc-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="3a5fc-130">Contém os resultados de resposta e as configurações de ausência temporária para um usuário.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="3a5fc-131">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="3a5fc-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3a5fc-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a5fc-132">Remarks</span></span>

<span data-ttu-id="3a5fc-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3a5fc-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a5fc-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3a5fc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a5fc-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a5fc-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a5fc-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a5fc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3a5fc-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3a5fc-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a5fc-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a5fc-138">Validation File</span></span>  <br/> |<span data-ttu-id="3a5fc-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a5fc-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a5fc-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3a5fc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a5fc-141">False</span><span class="sxs-lookup"><span data-stu-id="3a5fc-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a5fc-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="3a5fc-142">See also</span></span>



[<span data-ttu-id="3a5fc-143">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3a5fc-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="3a5fc-144">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3a5fc-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

