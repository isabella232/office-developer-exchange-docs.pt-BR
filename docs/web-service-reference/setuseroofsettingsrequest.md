---
title: SetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 628acf0b-3ebc-42f1-8ce2-7a02b4c8141f
description: O elemento SetUserOofSettingsRequest contém os argumentos usados para definir configurações de ausência temporária do usuário de uma caixa de correio.
ms.openlocfilehash: ed54bb1d066da7b15605fb81931a6ef75dfc61bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825474"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="9b5a9-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="9b5a9-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="9b5a9-104">O elemento **SetUserOofSettingsRequest** contém os argumentos usados para definir configurações de ausência temporária do usuário de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="9b5a9-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="9b5a9-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b5a9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9b5a9-106">Attributes and elements</span></span>

<span data-ttu-id="9b5a9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b5a9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9b5a9-108">Attributes</span></span>

<span data-ttu-id="9b5a9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b5a9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9b5a9-110">Child elements</span></span>

|<span data-ttu-id="9b5a9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b5a9-111">**Element**</span></span>|<span data-ttu-id="9b5a9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b5a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b5a9-113">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="9b5a9-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="9b5a9-114">Identifica o usuário de caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="9b5a9-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="9b5a9-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="9b5a9-116">Especifica as configurações de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b5a9-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9b5a9-117">Parent elements</span></span>

<span data-ttu-id="9b5a9-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9b5a9-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b5a9-119">Remarks</span></span>

<span data-ttu-id="9b5a9-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="9b5a9-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b5a9-121">Example</span></span>

<span data-ttu-id="9b5a9-122">O exemplo a seguir de uma solicitação de SetUserOofSettings define uma configuração de ausência temporária para dez dias.</span><span class="sxs-lookup"><span data-stu-id="9b5a9-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="9b5a9-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9b5a9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b5a9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b5a9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b5a9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9b5a9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9b5a9-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9b5a9-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9b5a9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9b5a9-127">Validation File</span></span>  <br/> |<span data-ttu-id="9b5a9-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b5a9-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b5a9-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9b5a9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b5a9-130">False</span><span class="sxs-lookup"><span data-stu-id="9b5a9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b5a9-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="9b5a9-131">See also</span></span>



[<span data-ttu-id="9b5a9-132">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="9b5a9-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

