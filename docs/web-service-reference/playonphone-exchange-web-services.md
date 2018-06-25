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
ms.openlocfilehash: 75493a31940ea609fd6cf454e91ca5881fb7e678
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824816"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="77f2c-103">PlayOnPhone (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="77f2c-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="77f2c-104">O elemento **PlayOnPhone** representa uma solicitação para ler um item em um telefone.</span><span class="sxs-lookup"><span data-stu-id="77f2c-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="77f2c-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="77f2c-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77f2c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="77f2c-106">Attributes and elements</span></span>

<span data-ttu-id="77f2c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77f2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77f2c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="77f2c-108">Attributes</span></span>

<span data-ttu-id="77f2c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77f2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77f2c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77f2c-110">Child elements</span></span>

|<span data-ttu-id="77f2c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77f2c-111">**Element**</span></span>|<span data-ttu-id="77f2c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77f2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77f2c-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="77f2c-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="77f2c-114">Representa o identificador de um item para tocar em um telefone.</span><span class="sxs-lookup"><span data-stu-id="77f2c-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="77f2c-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f2c-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="77f2c-116">DialString (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="77f2c-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="77f2c-117">Representa a cadeia de caracteres de discagem do número de telefone que é chamado para reproduzir um item por telefone.</span><span class="sxs-lookup"><span data-stu-id="77f2c-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="77f2c-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f2c-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77f2c-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77f2c-119">Parent elements</span></span>

<span data-ttu-id="77f2c-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77f2c-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77f2c-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="77f2c-121">Remarks</span></span>

<span data-ttu-id="77f2c-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="77f2c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77f2c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="77f2c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77f2c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="77f2c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77f2c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77f2c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="77f2c-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="77f2c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77f2c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77f2c-127">Validation File</span></span>  <br/> |<span data-ttu-id="77f2c-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77f2c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77f2c-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77f2c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="77f2c-130">False</span><span class="sxs-lookup"><span data-stu-id="77f2c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77f2c-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="77f2c-131">See also</span></span>



- [<span data-ttu-id="77f2c-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77f2c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

