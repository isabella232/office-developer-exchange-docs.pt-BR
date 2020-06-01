---
title: Mensagem (disponibilidade)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 1eec24dd-c981-41f4-a2f0-c51d43f1d7c0
description: O elemento Message contém a resposta de ausência temporária (OOF).
ms.openlocfilehash: 13d118422ccb5a2897c21b6d124f170bf461dbf6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467001"
---
# <a name="message-availability"></a><span data-ttu-id="d96f6-103">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d96f6-103">Message (Availability)</span></span>

<span data-ttu-id="d96f6-104">O elemento **Message** contém a resposta de ausência temporária (OOF).</span><span class="sxs-lookup"><span data-stu-id="d96f6-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="d96f6-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="d96f6-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d96f6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d96f6-106">Attributes and elements</span></span>

<span data-ttu-id="d96f6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d96f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d96f6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d96f6-108">Attributes</span></span>

<span data-ttu-id="d96f6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d96f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d96f6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d96f6-110">Child elements</span></span>

<span data-ttu-id="d96f6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d96f6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d96f6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d96f6-112">Parent elements</span></span>

|<span data-ttu-id="d96f6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d96f6-113">**Element**</span></span>|<span data-ttu-id="d96f6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d96f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d96f6-115">InternalReply</span><span class="sxs-lookup"><span data-stu-id="d96f6-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="d96f6-116">Contém a mensagem OOF enviada para outros usuários no domínio do remetente.</span><span class="sxs-lookup"><span data-stu-id="d96f6-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="d96f6-117">A seguir estão as possíveis expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d96f6-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="d96f6-118">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="d96f6-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="d96f6-119">Contém a mensagem OOF que é enviada para endereços fora do domínio do remetente.</span><span class="sxs-lookup"><span data-stu-id="d96f6-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="d96f6-120">A seguir estão as possíveis expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d96f6-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="d96f6-121">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="d96f6-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="d96f6-122">Contém uma mensagem OOF e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="d96f6-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d96f6-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d96f6-123">Text value</span></span>

<span data-ttu-id="d96f6-124">Um valor de texto é necessário para definir a mensagem OOF.</span><span class="sxs-lookup"><span data-stu-id="d96f6-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d96f6-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="d96f6-125">Remarks</span></span>

<span data-ttu-id="d96f6-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d96f6-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d96f6-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d96f6-127">Example</span></span>

<span data-ttu-id="d96f6-128">O exemplo a seguir de uma solicitação de [operação do SetUserOofSettings](setuseroofsettings-operation.md) define o [OofState](oofstate.md) como **habilitado**, define a duração de OOF como 10 dias e define as mensagens de ausência temporária interna e externa.</span><span class="sxs-lookup"><span data-stu-id="d96f6-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="d96f6-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d96f6-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d96f6-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="d96f6-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d96f6-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d96f6-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d96f6-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d96f6-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d96f6-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d96f6-133">Validation File</span></span>  <br/> |<span data-ttu-id="d96f6-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d96f6-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d96f6-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d96f6-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d96f6-136">False</span><span class="sxs-lookup"><span data-stu-id="d96f6-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d96f6-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d96f6-137">See also</span></span>

- [<span data-ttu-id="d96f6-138">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d96f6-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="d96f6-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d96f6-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

