---
title: PlayOnPhone (serviços Web do Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 486612be-470c-4f99-929a-f2b283e055c1
description: O elemento PlayOnPhone representa uma solicitação para ler um item em um telefone.
ms.openlocfilehash: e2c09a67255106ad9afddb86fa19b7a4a5762ee5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466245"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="e2030-103">PlayOnPhone (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="e2030-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="e2030-104">O elemento **PlayOnPhone** representa uma solicitação para ler um item em um telefone.</span><span class="sxs-lookup"><span data-stu-id="e2030-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="e2030-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="e2030-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2030-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e2030-106">Attributes and elements</span></span>

<span data-ttu-id="e2030-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2030-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2030-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2030-108">Attributes</span></span>

<span data-ttu-id="e2030-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2030-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2030-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2030-110">Child elements</span></span>

|<span data-ttu-id="e2030-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2030-111">**Element**</span></span>|<span data-ttu-id="e2030-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2030-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2030-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="e2030-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e2030-114">Representa o identificador de um item a ser tocado em um telefone.</span><span class="sxs-lookup"><span data-stu-id="e2030-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="e2030-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2030-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="e2030-116">Dialstring (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="e2030-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="e2030-117">Representa a cadeia de caracteres de discagem do número de telefone chamado para reproduzir um item por telefone.</span><span class="sxs-lookup"><span data-stu-id="e2030-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="e2030-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2030-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2030-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2030-119">Parent elements</span></span>

<span data-ttu-id="e2030-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2030-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2030-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2030-121">Remarks</span></span>

<span data-ttu-id="e2030-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e2030-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2030-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e2030-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2030-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2030-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2030-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2030-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e2030-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e2030-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2030-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2030-127">Validation File</span></span>  <br/> |<span data-ttu-id="e2030-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2030-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2030-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2030-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2030-130">False</span><span class="sxs-lookup"><span data-stu-id="e2030-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2030-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="e2030-131">See also</span></span>



- [<span data-ttu-id="e2030-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2030-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

