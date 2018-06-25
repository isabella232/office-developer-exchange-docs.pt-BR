---
title: Duração (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: O elemento de duração Especifica a duração em que o limite de status de ausência temporária será habilitado se o elemento OofState for definido como agendado.
ms.openlocfilehash: 62a5492372fd80173d58e965376b7c8c466825a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751945"
---
# <a name="duration-useroofsettings"></a><span data-ttu-id="d7414-103">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="d7414-103">Duration (UserOofSettings)</span></span>

<span data-ttu-id="d7414-104">O elemento de **duração** Especifica a duração em que o limite de status de ausência temporária será habilitado se o elemento [OofState](oofstate.md) for definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="d7414-104">The **Duration** element specifies the duration that the out of office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 <span data-ttu-id="d7414-105">**Duração**</span><span class="sxs-lookup"><span data-stu-id="d7414-105">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7414-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d7414-106">Attributes and elements</span></span>

<span data-ttu-id="d7414-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7414-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7414-108">Attributes</span></span>

<span data-ttu-id="d7414-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d7414-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7414-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7414-110">Child elements</span></span>

|<span data-ttu-id="d7414-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7414-111">**Element**</span></span>|<span data-ttu-id="d7414-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7414-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7414-113">StartTime</span><span class="sxs-lookup"><span data-stu-id="d7414-113">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="d7414-114">Representa o início do intervalo de tempo definido com um status de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d7414-114">Represents the start of the time span set with an OOF status.</span></span> <span data-ttu-id="d7414-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7414-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d7414-116">EndTime</span><span class="sxs-lookup"><span data-stu-id="d7414-116">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="d7414-117">Representa o fim do intervalo de tempo definido com um status de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d7414-117">Represents the end of the time span set with an OOF status.</span></span> <span data-ttu-id="d7414-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7414-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7414-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7414-119">Parent elements</span></span>

|<span data-ttu-id="d7414-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7414-120">**Element**</span></span>|<span data-ttu-id="d7414-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7414-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7414-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d7414-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="d7414-123">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d7414-123">Specifies the OOF settings.</span></span>  <br/><br/><span data-ttu-id="d7414-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d7414-124">The following is the XPath expression to this element:</span></span><br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="d7414-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="d7414-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="d7414-126">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="d7414-126">Contains the OOF settings.</span></span><br/><br/><span data-ttu-id="d7414-127">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d7414-127">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[<span data-ttu-id="d7414-128">Fora do escritório</span><span class="sxs-lookup"><span data-stu-id="d7414-128">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="d7414-129">Define a mensagem de resposta de ausência temporária e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d7414-129">Defines the Out of Office (OOF) response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7414-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="d7414-130">Remarks</span></span>

<span data-ttu-id="d7414-131">O tipo de **duração** também é o tipo para os elementos [DetailedSuggestionsWindow](detailedsuggestionswindow.md) [TimeWindow](timewindow.md)e [fora do escritório](outofoffice.md) .</span><span class="sxs-lookup"><span data-stu-id="d7414-131">The **Duration** type is also the type for the [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md), and [OutOfOffice](outofoffice.md) elements.</span></span> 
  
<span data-ttu-id="d7414-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7414-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d7414-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7414-133">Example</span></span>

<span data-ttu-id="d7414-134">O exemplo a seguir de uma solicitação de [operação SetUserOofSettings](setuseroofsettings-operation.md) define o [OofState](oofstate.md) como **habilitado**, as mensagens de ausência temporária internas e externas e define a duração de ausência temporária para 10 dias.</span><span class="sxs-lookup"><span data-stu-id="d7414-134">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, the internal and external OOF messages, and sets the duration of OOF for 10 days.</span></span>
  
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
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="d7414-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d7414-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7414-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7414-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7414-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7414-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d7414-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d7414-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7414-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7414-139">Validation File</span></span>  <br/> |<span data-ttu-id="d7414-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d7414-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7414-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d7414-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7414-142">False</span><span class="sxs-lookup"><span data-stu-id="d7414-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7414-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="d7414-143">See also</span></span>

- [<span data-ttu-id="d7414-144">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d7414-144">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)  
- [<span data-ttu-id="d7414-145">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d7414-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

