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
description: O elemento OofSettings contém as configurações de ausência temporária (OOF).
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467190"
---
# <a name="oofsettings"></a><span data-ttu-id="3adf8-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3adf8-103">OofSettings</span></span>

<span data-ttu-id="3adf8-104">O elemento **OofSettings** contém as configurações de ausência temporária (OOF).</span><span class="sxs-lookup"><span data-stu-id="3adf8-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="3adf8-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3adf8-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="3adf8-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3adf8-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="3adf8-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="3adf8-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3adf8-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3adf8-108">Attributes and elements</span></span>

<span data-ttu-id="3adf8-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3adf8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3adf8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3adf8-110">Attributes</span></span>

<span data-ttu-id="3adf8-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3adf8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3adf8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3adf8-112">Child elements</span></span>

|<span data-ttu-id="3adf8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3adf8-113">**Element**</span></span>|<span data-ttu-id="3adf8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3adf8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3adf8-115">OofState</span><span class="sxs-lookup"><span data-stu-id="3adf8-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="3adf8-116">Contém o estado de ausência temporária do usuário.</span><span class="sxs-lookup"><span data-stu-id="3adf8-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="3adf8-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="3adf8-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="3adf8-118">Contém um valor que determina a quem mensagens externas OOF são enviadas.</span><span class="sxs-lookup"><span data-stu-id="3adf8-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="3adf8-119">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="3adf8-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="3adf8-120">Contém a duração para a qual o status de ausência temporária é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="3adf8-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="3adf8-121">Se o elemento [OofState](oofstate.md) estiver definido como **Enabled** ou **Disabled**, o valor desse elemento será ignorado.</span><span class="sxs-lookup"><span data-stu-id="3adf8-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="3adf8-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="3adf8-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="3adf8-123">Contém a resposta de ausência temporária enviada a outros usuários no domínio do usuário ou domínio confiável.</span><span class="sxs-lookup"><span data-stu-id="3adf8-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="3adf8-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="3adf8-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="3adf8-125">Contém a resposta de ausência temporária enviada para endereços fora do domínio do destinatário ou domínios confiáveis.</span><span class="sxs-lookup"><span data-stu-id="3adf8-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3adf8-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3adf8-126">Parent elements</span></span>

|<span data-ttu-id="3adf8-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3adf8-127">**Element**</span></span>|<span data-ttu-id="3adf8-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3adf8-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3adf8-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3adf8-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="3adf8-130">Contém os resultados da resposta e as configurações de ausência temporária de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3adf8-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="3adf8-131">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3adf8-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3adf8-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="3adf8-132">Remarks</span></span>

<span data-ttu-id="3adf8-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3adf8-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3adf8-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3adf8-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3adf8-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="3adf8-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3adf8-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3adf8-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3adf8-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3adf8-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3adf8-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3adf8-138">Validation File</span></span>  <br/> |<span data-ttu-id="3adf8-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3adf8-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3adf8-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3adf8-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3adf8-141">False</span><span class="sxs-lookup"><span data-stu-id="3adf8-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3adf8-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="3adf8-142">See also</span></span>



[<span data-ttu-id="3adf8-143">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3adf8-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="3adf8-144">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3adf8-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

