---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: O elemento UsePOPAuth indica se as informações de autenticação fornecidas para um tipo de conta POP3 também são usadas para SMTP (Simple Mail Transfer Protocol).
ms.openlocfilehash: 8d5bfffaab31c382ad43915e18b8a7a2b2737c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466504"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="774d7-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="774d7-104">O elemento **UsePOPAuth** indica se as informações de autenticação fornecidas para um tipo de conta POP3 também são usadas para SMTP (Simple Mail Transfer Protocol).</span><span class="sxs-lookup"><span data-stu-id="774d7-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="774d7-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="774d7-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="774d7-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="774d7-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="774d7-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="774d7-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="774d7-110">Attributes and elements</span></span>

<span data-ttu-id="774d7-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="774d7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="774d7-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="774d7-112">Attributes</span></span>

<span data-ttu-id="774d7-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="774d7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="774d7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="774d7-114">Child elements</span></span>

<span data-ttu-id="774d7-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="774d7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="774d7-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="774d7-116">Parent elements</span></span>

|<span data-ttu-id="774d7-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="774d7-117">**Element**</span></span>|<span data-ttu-id="774d7-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="774d7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="774d7-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="774d7-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="774d7-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="774d7-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="774d7-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="774d7-121">Text value</span></span>

<span data-ttu-id="774d7-122">O valor de texto indica se as informações de autenticação fornecidas para um tipo de conta POP3 também são usadas para SMTP.</span><span class="sxs-lookup"><span data-stu-id="774d7-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="774d7-123">Os valores possíveis estão **ativados** e **desativados**.</span><span class="sxs-lookup"><span data-stu-id="774d7-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="774d7-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="774d7-124">Remarks</span></span>

<span data-ttu-id="774d7-125">O elemento **UsePOPAuth** é usado apenas quando o [tipo (POX)](type-pox.md) é SMTP.</span><span class="sxs-lookup"><span data-stu-id="774d7-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="774d7-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="774d7-126">See also</span></span>



[<span data-ttu-id="774d7-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="774d7-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

