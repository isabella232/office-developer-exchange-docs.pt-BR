---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: O elemento InternalReply contém o limite da resposta de ausência temporária enviada para outros usuários no domínio ou os domínios confiáveis do usuário.
ms.openlocfilehash: ac5e9eadac7f45c233007ffb05f4d2430875ec52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823955"
---
# <a name="internalreply"></a><span data-ttu-id="d36de-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="d36de-103">InternalReply</span></span>

<span data-ttu-id="d36de-104">O elemento **InternalReply** contém o limite da resposta de ausência temporária enviada para outros usuários no domínio ou os domínios confiáveis do usuário.</span><span class="sxs-lookup"><span data-stu-id="d36de-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="d36de-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="d36de-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d36de-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d36de-106">Attributes and elements</span></span>

<span data-ttu-id="d36de-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d36de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d36de-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d36de-108">Attributes</span></span>

|<span data-ttu-id="d36de-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="d36de-109">**Attribute**</span></span>|<span data-ttu-id="d36de-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d36de-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d36de-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="d36de-111">xml:lang</span></span>  <br/> |<span data-ttu-id="d36de-112">Especifica o idioma usado na mensagem **InternalReply** .</span><span class="sxs-lookup"><span data-stu-id="d36de-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="d36de-113">Os valores possíveis desse atributo são definidos por IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="d36de-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d36de-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d36de-114">Child elements</span></span>

|<span data-ttu-id="d36de-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d36de-115">**Element**</span></span>|<span data-ttu-id="d36de-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d36de-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d36de-117">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d36de-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="d36de-118">Contém a resposta de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d36de-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d36de-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d36de-119">Parent elements</span></span>

|<span data-ttu-id="d36de-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d36de-120">**Element**</span></span>|<span data-ttu-id="d36de-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d36de-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d36de-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d36de-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="d36de-123">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d36de-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="d36de-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d36de-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="d36de-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d36de-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="d36de-126">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d36de-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="d36de-127">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d36de-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d36de-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="d36de-128">Remarks</span></span>

<span data-ttu-id="d36de-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d36de-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d36de-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d36de-130">Example</span></span>

<span data-ttu-id="d36de-131">O exemplo a seguir de uma solicitação de SetUserOofSettings define o [OofState](oofstate.md) como **habilitada**, define a duração de ausência temporária para 10 dias e define as mensagens de ausência temporária internas e externas.</span><span class="sxs-lookup"><span data-stu-id="d36de-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
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

## <a name="element-information"></a><span data-ttu-id="d36de-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d36de-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d36de-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="d36de-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d36de-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d36de-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d36de-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d36de-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d36de-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d36de-136">Validation File</span></span>  <br/> |<span data-ttu-id="d36de-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d36de-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d36de-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d36de-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d36de-139">False</span><span class="sxs-lookup"><span data-stu-id="d36de-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d36de-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="d36de-140">See also</span></span>



[<span data-ttu-id="d36de-141">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d36de-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="d36de-142">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d36de-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

