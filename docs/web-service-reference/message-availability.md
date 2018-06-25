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
description: O elemento de mensagem contém o de resposta de ausência temporária.
ms.openlocfilehash: 9facd04767fdcc0fd9dfd84fc6badb1a7633d2b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824452"
---
# <a name="message-availability"></a><span data-ttu-id="daef8-103">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="daef8-103">Message (Availability)</span></span>

<span data-ttu-id="daef8-104">O elemento de **mensagem** contém o de resposta de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="daef8-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="daef8-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="daef8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="daef8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="daef8-106">Attributes and elements</span></span>

<span data-ttu-id="daef8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="daef8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="daef8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="daef8-108">Attributes</span></span>

<span data-ttu-id="daef8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="daef8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="daef8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="daef8-110">Child elements</span></span>

<span data-ttu-id="daef8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="daef8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="daef8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="daef8-112">Parent elements</span></span>

|<span data-ttu-id="daef8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="daef8-113">**Element**</span></span>|<span data-ttu-id="daef8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="daef8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="daef8-115">InternalReply</span><span class="sxs-lookup"><span data-stu-id="daef8-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="daef8-116">Contém a mensagem de ausência temporária enviada para outros usuários no domínio do remetente.</span><span class="sxs-lookup"><span data-stu-id="daef8-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="daef8-117">A seguir estão as expressões XPath possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="daef8-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="daef8-118">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="daef8-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="daef8-119">Contém a mensagem de ausência temporária que é enviada para endereços fora do domínio do remetente.</span><span class="sxs-lookup"><span data-stu-id="daef8-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="daef8-120">A seguir estão as expressões XPath possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="daef8-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="daef8-121">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="daef8-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="daef8-122">Contém uma mensagem de ausência temporária e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="daef8-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="daef8-123">Text value</span><span class="sxs-lookup"><span data-stu-id="daef8-123">Text value</span></span>

<span data-ttu-id="daef8-124">Um valor de texto é obrigatório para definir a mensagem de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="daef8-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="daef8-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="daef8-125">Remarks</span></span>

<span data-ttu-id="daef8-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="daef8-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="daef8-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daef8-127">Example</span></span>

<span data-ttu-id="daef8-128">O exemplo a seguir de uma solicitação de [operação SetUserOofSettings](setuseroofsettings-operation.md) define o [OofState](oofstate.md) como **habilitada**, define a duração de ausência temporária para 10 dias e define as mensagens de ausência temporária internas e externas.</span><span class="sxs-lookup"><span data-stu-id="daef8-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="daef8-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="daef8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="daef8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="daef8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="daef8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="daef8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="daef8-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="daef8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="daef8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="daef8-133">Validation File</span></span>  <br/> |<span data-ttu-id="daef8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="daef8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="daef8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="daef8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="daef8-136">False</span><span class="sxs-lookup"><span data-stu-id="daef8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="daef8-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="daef8-137">See also</span></span>

- [<span data-ttu-id="daef8-138">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="daef8-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="daef8-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="daef8-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

