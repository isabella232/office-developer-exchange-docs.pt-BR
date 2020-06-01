---
title: GetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 15dea99c-7f5d-4af1-82ff-4255127fe567
description: O elemento GetUserOofSettingsRequest é o elemento raiz que contém os argumentos usados para obter as configurações de ausência temporária (OOF) de um usuário de caixa de correio.
ms.openlocfilehash: f515e8cf016d3aff6c652ae92a0da71a8f0a5f6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457827"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="6ce1f-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="6ce1f-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="6ce1f-104">O elemento **GetUserOofSettingsRequest** é o elemento raiz que contém os argumentos usados para obter as configurações de ausência temporária (OOF) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ce1f-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="6ce1f-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="6ce1f-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ce1f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6ce1f-106">Attributes and elements</span></span>

<span data-ttu-id="6ce1f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ce1f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ce1f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ce1f-108">Attributes</span></span>

<span data-ttu-id="6ce1f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ce1f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ce1f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ce1f-110">Child elements</span></span>

|<span data-ttu-id="6ce1f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ce1f-111">**Element**</span></span>|<span data-ttu-id="6ce1f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ce1f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ce1f-113">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="6ce1f-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="6ce1f-114">Identifica o usuário de caixa de correio para uma solicitação de SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="6ce1f-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ce1f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ce1f-115">Parent elements</span></span>

<span data-ttu-id="6ce1f-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ce1f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ce1f-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ce1f-117">Remarks</span></span>

<span data-ttu-id="6ce1f-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6ce1f-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6ce1f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ce1f-119">Example</span></span>

<span data-ttu-id="6ce1f-120">Veja a seguir um exemplo de uma solicitação GetUserOofSettings que obtém as informações de OOF de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="6ce1f-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="6ce1f-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6ce1f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ce1f-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ce1f-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ce1f-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ce1f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6ce1f-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6ce1f-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ce1f-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ce1f-125">Validation File</span></span>  <br/> |<span data-ttu-id="6ce1f-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6ce1f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ce1f-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6ce1f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ce1f-128">False</span><span class="sxs-lookup"><span data-stu-id="6ce1f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ce1f-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ce1f-129">See also</span></span>



[<span data-ttu-id="6ce1f-130">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6ce1f-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

