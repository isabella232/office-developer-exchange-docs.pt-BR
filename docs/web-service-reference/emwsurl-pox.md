---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: O elemento EmwsUrl Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752038"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="62a1c-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="62a1c-104">O elemento **EmwsUrl** Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="62a1c-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="62a1c-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="62a1c-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="62a1c-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="62a1c-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="62a1c-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="62a1c-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="62a1c-110">Attributes and elements</span></span>

<span data-ttu-id="62a1c-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="62a1c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62a1c-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="62a1c-112">Attributes</span></span>

<span data-ttu-id="62a1c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="62a1c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62a1c-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="62a1c-114">Child elements</span></span>

<span data-ttu-id="62a1c-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="62a1c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="62a1c-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="62a1c-116">Parent elements</span></span>

|<span data-ttu-id="62a1c-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="62a1c-117">**Element**</span></span>|<span data-ttu-id="62a1c-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="62a1c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62a1c-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="62a1c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="62a1c-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="62a1c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="62a1c-121">Text value</span><span class="sxs-lookup"><span data-stu-id="62a1c-121">Text value</span></span>

<span data-ttu-id="62a1c-122">O valor de texto representa a URL do ponto de extremidade EWS para o usuário.</span><span class="sxs-lookup"><span data-stu-id="62a1c-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="62a1c-123">É equivalente ao elemento [EwsUrl POX ()](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="62a1c-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="62a1c-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="62a1c-124">Remarks</span></span>

<span data-ttu-id="62a1c-125">O **EmwsUrl** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="62a1c-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="62a1c-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="62a1c-126">See also</span></span>

- [<span data-ttu-id="62a1c-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="62a1c-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

