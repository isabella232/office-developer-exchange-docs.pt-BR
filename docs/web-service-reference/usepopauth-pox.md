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
description: O elemento UsePOPAuth indica se as informações de autenticação que são fornecidas para um tipo de POP3 da conta também são usadas para SMTP Simple Mail Transfer Protocol ().
ms.openlocfilehash: be03568d697b1f5461d49dba388a1d3f1008a67e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837964"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="f0830-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="f0830-104">O elemento **UsePOPAuth** indica se as informações de autenticação que são fornecidas para um tipo de POP3 da conta também são usadas para SMTP Simple Mail Transfer Protocol ().</span><span class="sxs-lookup"><span data-stu-id="f0830-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="f0830-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f0830-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f0830-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f0830-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f0830-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f0830-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f0830-110">Attributes and elements</span></span>

<span data-ttu-id="f0830-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f0830-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0830-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="f0830-112">Attributes</span></span>

<span data-ttu-id="f0830-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f0830-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0830-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f0830-114">Child elements</span></span>

<span data-ttu-id="f0830-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f0830-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0830-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f0830-116">Parent elements</span></span>

|<span data-ttu-id="f0830-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f0830-117">**Element**</span></span>|<span data-ttu-id="f0830-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0830-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0830-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="f0830-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f0830-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f0830-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0830-121">Text value</span><span class="sxs-lookup"><span data-stu-id="f0830-121">Text value</span></span>

<span data-ttu-id="f0830-122">O valor de texto indica se as informações de autenticação que são fornecidas para um tipo de POP3 da conta também são usadas para SMTP.</span><span class="sxs-lookup"><span data-stu-id="f0830-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="f0830-123">Os valores possíveis são **Ativar** e **Desativar**.</span><span class="sxs-lookup"><span data-stu-id="f0830-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0830-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0830-124">Remarks</span></span>

<span data-ttu-id="f0830-125">O elemento **UsePOPAuth** é usado apenas quando o [Tipo POX ()](type-pox.md) é SMTP.</span><span class="sxs-lookup"><span data-stu-id="f0830-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f0830-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="f0830-126">See also</span></span>



[<span data-ttu-id="f0830-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="f0830-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

