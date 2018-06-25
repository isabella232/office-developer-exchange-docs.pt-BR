---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: O elemento OofState é usado para obter ou definir o estado de fora do escritório (OOF) do usuário.
ms.openlocfilehash: f97c050aec102b384fa4d98e6dee43befd4dc9ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824651"
---
# <a name="oofstate"></a><span data-ttu-id="75266-103">OofState</span><span class="sxs-lookup"><span data-stu-id="75266-103">OofState</span></span>

<span data-ttu-id="75266-104">O elemento **OofState** é usado para obter ou definir o estado de fora do escritório (OOF) do usuário.</span><span class="sxs-lookup"><span data-stu-id="75266-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="75266-105">**OofState**</span><span class="sxs-lookup"><span data-stu-id="75266-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75266-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="75266-106">Attributes and elements</span></span>

<span data-ttu-id="75266-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="75266-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75266-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="75266-108">Attributes</span></span>

<span data-ttu-id="75266-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="75266-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75266-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="75266-110">Child elements</span></span>

<span data-ttu-id="75266-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="75266-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75266-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="75266-112">Parent elements</span></span>

|<span data-ttu-id="75266-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="75266-113">**Element**</span></span>|<span data-ttu-id="75266-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="75266-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75266-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="75266-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="75266-116">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="75266-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="75266-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="75266-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="75266-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="75266-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="75266-119">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="75266-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="75266-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="75266-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75266-121">Text value</span><span class="sxs-lookup"><span data-stu-id="75266-121">Text value</span></span>

<span data-ttu-id="75266-122">Um valor de texto é necessário para o elemento **OofState** .</span><span class="sxs-lookup"><span data-stu-id="75266-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="75266-123">A lista a seguir contém os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="75266-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="75266-124">**Desabilitado**</span><span class="sxs-lookup"><span data-stu-id="75266-124">**Disabled**</span></span>
    
- <span data-ttu-id="75266-125">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="75266-125">**Enabled**</span></span>
    
- <span data-ttu-id="75266-126">**Agendado**</span><span class="sxs-lookup"><span data-stu-id="75266-126">**Scheduled**</span></span>
    
<span data-ttu-id="75266-127">Um valor **agendado** indica que o status de ausência temporária está definido como **habilitada** durante um período de tempo identificado pelo elemento [duração (UserOofSettings)](duration-useroofsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="75266-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75266-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="75266-128">Remarks</span></span>

<span data-ttu-id="75266-129">Esse elemento é necessário em ambos a SetUsersOofSettingRequest e a mensagem GetUserOofSettingResponse.</span><span class="sxs-lookup"><span data-stu-id="75266-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="75266-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="75266-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="75266-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75266-131">Example</span></span>

<span data-ttu-id="75266-132">O exemplo a seguir de uma solicitação de SetUserOofSettings permite que o **OofState**.</span><span class="sxs-lookup"><span data-stu-id="75266-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="75266-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="75266-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75266-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="75266-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75266-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="75266-135">Schema Name</span></span>  <br/> |<span data-ttu-id="75266-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="75266-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="75266-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="75266-137">Validation File</span></span>  <br/> |<span data-ttu-id="75266-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="75266-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75266-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="75266-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="75266-140">False</span><span class="sxs-lookup"><span data-stu-id="75266-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75266-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="75266-141">See also</span></span>



[<span data-ttu-id="75266-142">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="75266-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="75266-143">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="75266-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

