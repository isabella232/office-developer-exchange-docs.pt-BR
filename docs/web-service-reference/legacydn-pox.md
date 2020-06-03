---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: O elemento LegacyDN identifica a caixa de correio de um usuário com o nome diferenciado herdado.
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526379"
---
# <a name="legacydn-pox"></a><span data-ttu-id="56431-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="56431-103">LegacyDN (POX)</span></span>

<span data-ttu-id="56431-104">O elemento **LegacyDN** identifica a caixa de correio de um usuário com o nome diferenciado herdado.</span><span class="sxs-lookup"><span data-stu-id="56431-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="56431-105">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="56431-105">Attributes and elements</span></span>

<span data-ttu-id="56431-106">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="56431-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56431-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="56431-107">Attributes</span></span>

<span data-ttu-id="56431-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56431-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56431-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="56431-109">Child elements</span></span>

<span data-ttu-id="56431-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56431-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56431-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="56431-111">Parent elements</span></span>

|<span data-ttu-id="56431-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="56431-112">**Element**</span></span>|<span data-ttu-id="56431-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56431-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56431-114">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="56431-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="56431-115">Contém a solicitação para o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="56431-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="56431-116">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="56431-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="56431-117">Fornece informações específicas do usuário.</span><span class="sxs-lookup"><span data-stu-id="56431-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56431-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="56431-118">Text value</span></span>

<span data-ttu-id="56431-119">O valor de texto representa o endereço de email herdado de um usuário.</span><span class="sxs-lookup"><span data-stu-id="56431-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56431-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="56431-120">Remarks</span></span>

<span data-ttu-id="56431-121">O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é um elemento alternativo para uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="56431-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="56431-122">Ele é usado quando uma caixa de correio existe em um computador que esteja executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="56431-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="56431-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="56431-123">See also</span></span>

- [<span data-ttu-id="56431-124">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="56431-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

