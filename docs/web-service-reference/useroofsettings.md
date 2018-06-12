---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: O elemento UserOofSettings Especifica as configurações de fora do escritório (OOF).
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837993"
---
# <a name="useroofsettings"></a><span data-ttu-id="09d86-103">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="09d86-103">UserOofSettings</span></span>

<span data-ttu-id="09d86-104">O elemento **UserOofSettings** Especifica as configurações de fora do escritório (OOF).</span><span class="sxs-lookup"><span data-stu-id="09d86-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="09d86-105">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="09d86-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="09d86-106">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="09d86-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="09d86-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="09d86-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09d86-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="09d86-108">Attributes and elements</span></span>

<span data-ttu-id="09d86-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="09d86-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09d86-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="09d86-110">Attributes</span></span>

<span data-ttu-id="09d86-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="09d86-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09d86-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="09d86-112">Child elements</span></span>

|<span data-ttu-id="09d86-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="09d86-113">**Element**</span></span>|<span data-ttu-id="09d86-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="09d86-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09d86-115">OofState</span><span class="sxs-lookup"><span data-stu-id="09d86-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="09d86-116">Define o estado de ausência temporária do usuário.</span><span class="sxs-lookup"><span data-stu-id="09d86-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="09d86-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="09d86-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="09d86-118">Define ou contém um valor que determina a quem as mensagens de ausência temporária externas são enviadas.</span><span class="sxs-lookup"><span data-stu-id="09d86-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="09d86-119">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="09d86-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="09d86-120">Especifica a duração em que o status de ausência temporária está ativado se o elemento [OofState](oofstate.md) for definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="09d86-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="09d86-121">Se o elemento [OofState](oofstate.md) for definido como **habilitado** ou **desabilitado**, o valor deste elemento será ignorado.</span><span class="sxs-lookup"><span data-stu-id="09d86-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="09d86-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="09d86-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="09d86-123">Contém a resposta de ausência temporária enviada para outros usuários no domínio ou os domínios confiáveis do usuário.</span><span class="sxs-lookup"><span data-stu-id="09d86-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="09d86-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="09d86-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="09d86-125">Contém a resposta de ausência temporária enviada para endereços fora do domínio ou os domínios confiáveis do destinatário.</span><span class="sxs-lookup"><span data-stu-id="09d86-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09d86-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="09d86-126">Parent elements</span></span>

|<span data-ttu-id="09d86-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="09d86-127">**Element**</span></span>|<span data-ttu-id="09d86-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="09d86-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09d86-129">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="09d86-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="09d86-130">Contém os argumentos usados para definir configurações de ausência temporária e mensagens de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="09d86-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="09d86-131">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="09d86-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="09d86-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="09d86-132">Remarks</span></span>

<span data-ttu-id="09d86-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="09d86-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="09d86-134">Example</span><span class="sxs-lookup"><span data-stu-id="09d86-134">Example</span></span>

<span data-ttu-id="09d86-135">O exemplo a seguir de uma solicitação de SetUserOofSettings define o OoFState como **habilitada**, define a duração de ausência temporária para 10 dias e define as mensagens de ausência temporária internas e externas.</span><span class="sxs-lookup"><span data-stu-id="09d86-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="09d86-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="09d86-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09d86-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="09d86-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09d86-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="09d86-138">Schema Name</span></span>  <br/> |<span data-ttu-id="09d86-139">esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="09d86-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="09d86-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="09d86-140">Validation File</span></span>  <br/> |<span data-ttu-id="09d86-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="09d86-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09d86-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="09d86-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="09d86-143">False</span><span class="sxs-lookup"><span data-stu-id="09d86-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09d86-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="09d86-144">See also</span></span>

- [<span data-ttu-id="09d86-145">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="09d86-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

