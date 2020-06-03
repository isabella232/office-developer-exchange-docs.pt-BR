---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: O elemento EmwsUrl especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email.
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530667"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="bc6b2-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="bc6b2-104">O elemento **EmwsUrl** especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="bc6b2-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="bc6b2-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="bc6b2-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="bc6b2-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="bc6b2-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="bc6b2-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="bc6b2-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bc6b2-110">Attributes and elements</span></span>

<span data-ttu-id="bc6b2-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bc6b2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc6b2-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="bc6b2-112">Attributes</span></span>

<span data-ttu-id="bc6b2-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc6b2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc6b2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bc6b2-114">Child elements</span></span>

<span data-ttu-id="bc6b2-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bc6b2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc6b2-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bc6b2-116">Parent elements</span></span>

|<span data-ttu-id="bc6b2-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bc6b2-117">**Element**</span></span>|<span data-ttu-id="bc6b2-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bc6b2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc6b2-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="bc6b2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="bc6b2-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="bc6b2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc6b2-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bc6b2-121">Text value</span></span>

<span data-ttu-id="bc6b2-122">O valor de texto representa a URL do ponto de extremidade do EWS para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bc6b2-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="bc6b2-123">É equivalente ao elemento [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="bc6b2-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bc6b2-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="bc6b2-124">Remarks</span></span>

<span data-ttu-id="bc6b2-125">O elemento **EmwsUrl** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="bc6b2-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bc6b2-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc6b2-126">See also</span></span>

- [<span data-ttu-id="bc6b2-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="bc6b2-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

