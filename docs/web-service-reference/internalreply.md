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
description: O elemento InternalReply contém a resposta de ausência temporária (OOF) enviada a outros usuários no domínio ou domínios confiáveis do usuário.
ms.openlocfilehash: 24c278ebd3acf83e87fbf72650eb3d5d438d5c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465580"
---
# <a name="internalreply"></a><span data-ttu-id="d69e7-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="d69e7-103">InternalReply</span></span>

<span data-ttu-id="d69e7-104">O elemento **InternalReply** contém a resposta de ausência temporária (OOF) enviada a outros usuários no domínio ou domínios confiáveis do usuário.</span><span class="sxs-lookup"><span data-stu-id="d69e7-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="d69e7-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="d69e7-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d69e7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d69e7-106">Attributes and elements</span></span>

<span data-ttu-id="d69e7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d69e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d69e7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d69e7-108">Attributes</span></span>

|<span data-ttu-id="d69e7-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d69e7-109">**Attribute**</span></span>|<span data-ttu-id="d69e7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d69e7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d69e7-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="d69e7-111">xml:lang</span></span>  <br/> |<span data-ttu-id="d69e7-112">Especifica o idioma usado na mensagem **InternalReply** .</span><span class="sxs-lookup"><span data-stu-id="d69e7-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="d69e7-113">Os valores possíveis desse atributo são definidos pela IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="d69e7-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d69e7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d69e7-114">Child elements</span></span>

|<span data-ttu-id="d69e7-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d69e7-115">**Element**</span></span>|<span data-ttu-id="d69e7-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d69e7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d69e7-117">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d69e7-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="d69e7-118">Contém a resposta de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d69e7-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d69e7-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d69e7-119">Parent elements</span></span>

|<span data-ttu-id="d69e7-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d69e7-120">**Element**</span></span>|<span data-ttu-id="d69e7-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d69e7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d69e7-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d69e7-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="d69e7-123">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d69e7-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="d69e7-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d69e7-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="d69e7-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d69e7-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="d69e7-126">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d69e7-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="d69e7-127">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d69e7-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d69e7-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="d69e7-128">Remarks</span></span>

<span data-ttu-id="d69e7-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d69e7-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d69e7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d69e7-130">Example</span></span>

<span data-ttu-id="d69e7-131">O exemplo a seguir de uma solicitação SetUserOofSettings define o [OofState](oofstate.md) como **habilitado**, define a duração de OOF por 10 dias e define as mensagens externas e externa OOF.</span><span class="sxs-lookup"><span data-stu-id="d69e7-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="d69e7-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d69e7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d69e7-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="d69e7-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d69e7-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d69e7-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d69e7-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d69e7-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d69e7-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d69e7-136">Validation File</span></span>  <br/> |<span data-ttu-id="d69e7-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d69e7-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d69e7-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d69e7-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d69e7-139">False</span><span class="sxs-lookup"><span data-stu-id="d69e7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d69e7-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="d69e7-140">See also</span></span>



[<span data-ttu-id="d69e7-141">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d69e7-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="d69e7-142">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d69e7-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

