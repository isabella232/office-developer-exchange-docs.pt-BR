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
description: O GetUserOofSettingsRequest é o elemento raiz que contém os argumentos usados para fazer configurações de ausência temporária do usuário a uma caixa de correio.
ms.openlocfilehash: e64818961283f90e447e2044cf7f918eccd21f06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823692"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="98ea4-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="98ea4-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="98ea4-104">O **GetUserOofSettingsRequest** é o elemento raiz que contém os argumentos usados para fazer configurações de ausência temporária do usuário a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="98ea4-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="98ea4-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="98ea4-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98ea4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="98ea4-106">Attributes and elements</span></span>

<span data-ttu-id="98ea4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="98ea4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98ea4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="98ea4-108">Attributes</span></span>

<span data-ttu-id="98ea4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98ea4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98ea4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="98ea4-110">Child elements</span></span>

|<span data-ttu-id="98ea4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="98ea4-111">**Element**</span></span>|<span data-ttu-id="98ea4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98ea4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98ea4-113">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="98ea4-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="98ea4-114">Identifica o usuário de caixa de correio para uma solicitação SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="98ea4-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="98ea4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="98ea4-115">Parent elements</span></span>

<span data-ttu-id="98ea4-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98ea4-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98ea4-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="98ea4-117">Remarks</span></span>

<span data-ttu-id="98ea4-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="98ea4-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="98ea4-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98ea4-119">Example</span></span>

<span data-ttu-id="98ea4-120">O exemplo a seguir é um exemplo de uma solicitação de GetUserOofSettings que obtém informações de ausência temporária de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="98ea4-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="98ea4-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="98ea4-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98ea4-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="98ea4-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98ea4-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="98ea4-123">Schema Name</span></span>  <br/> |<span data-ttu-id="98ea4-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="98ea4-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98ea4-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="98ea4-125">Validation File</span></span>  <br/> |<span data-ttu-id="98ea4-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98ea4-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98ea4-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="98ea4-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="98ea4-128">False</span><span class="sxs-lookup"><span data-stu-id="98ea4-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98ea4-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="98ea4-129">See also</span></span>



[<span data-ttu-id="98ea4-130">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="98ea4-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

