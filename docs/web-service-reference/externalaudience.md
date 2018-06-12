---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: O elemento ExternalAudience define ou contém um valor que determina a quem as mensagens de ausência temporária externas são enviadas.
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752194"
---
# <a name="externalaudience"></a><span data-ttu-id="8ac1f-103">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="8ac1f-103">ExternalAudience</span></span>

<span data-ttu-id="8ac1f-104">O elemento **ExternalAudience** define ou contém um valor que determina a quem as mensagens de ausência temporária externas são enviadas.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="8ac1f-105">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ac1f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8ac1f-106">Attributes and elements</span></span>

<span data-ttu-id="8ac1f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ac1f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ac1f-108">Attributes</span></span>

<span data-ttu-id="8ac1f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ac1f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ac1f-110">Child elements</span></span>

<span data-ttu-id="8ac1f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ac1f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ac1f-112">Parent elements</span></span>

|<span data-ttu-id="8ac1f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-113">**Element**</span></span>|<span data-ttu-id="8ac1f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ac1f-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac1f-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="8ac1f-116">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="8ac1f-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="8ac1f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="8ac1f-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac1f-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="8ac1f-119">Contém as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="8ac1f-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="8ac1f-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ac1f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="8ac1f-121">Text value</span></span>

<span data-ttu-id="8ac1f-122">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-122">A text value is required for this element.</span></span> <span data-ttu-id="8ac1f-123">A tabela a seguir lista os valores possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="8ac1f-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-124">**Value**</span></span>|<span data-ttu-id="8ac1f-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8ac1f-126">**None**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-126">**None**</span></span> <br/> |<span data-ttu-id="8ac1f-127">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário não receberá uma resposta de mensagem de ausência temporária externa.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="8ac1f-128">**Conhecidos**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-128">**Known**</span></span> <br/> |<span data-ttu-id="8ac1f-129">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa apenas se o remetente está no Exchange do usuário armazenam a lista de contatos.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="8ac1f-130">**All**</span><span class="sxs-lookup"><span data-stu-id="8ac1f-130">**All**</span></span> <br/> |<span data-ttu-id="8ac1f-131">Remetentes de email fora da organização do usuário da caixa de correio que enviar mensagens para o usuário receberá uma resposta de mensagem de ausência temporária externa.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8ac1f-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8ac1f-132">Remarks</span></span>

<span data-ttu-id="8ac1f-133">Esse elemento compartilha o mesmo tipo de elemento [AllowExternalOof](allowexternaloof.md) .</span><span class="sxs-lookup"><span data-stu-id="8ac1f-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="8ac1f-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="8ac1f-135">Example</span><span class="sxs-lookup"><span data-stu-id="8ac1f-135">Example</span></span>

<span data-ttu-id="8ac1f-136">O exemplo a seguir de uma solicitação de SetUserOofSettings define o OoFState como **habilitada**, define o público externo para **todos os**, define a duração de ausência temporária para 10 dias e define as mensagens de ausência temporária internas e externas.</span><span class="sxs-lookup"><span data-stu-id="8ac1f-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="8ac1f-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8ac1f-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ac1f-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ac1f-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ac1f-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8ac1f-139">Schema Name</span></span>  <br/> |<span data-ttu-id="8ac1f-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8ac1f-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ac1f-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8ac1f-141">Validation File</span></span>  <br/> |<span data-ttu-id="8ac1f-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ac1f-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ac1f-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8ac1f-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ac1f-144">False</span><span class="sxs-lookup"><span data-stu-id="8ac1f-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ac1f-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="8ac1f-145">See also</span></span>



[<span data-ttu-id="8ac1f-146">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac1f-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="8ac1f-147">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ac1f-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

