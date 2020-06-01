---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: O elemento DomainRequired indica se o domínio é necessário para autenticação.
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461321"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="41b85-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-103">DomainRequired (POX)</span></span>

<span data-ttu-id="41b85-104">O elemento **DomainRequired** indica se o domínio é necessário para autenticação.</span><span class="sxs-lookup"><span data-stu-id="41b85-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="41b85-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="41b85-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="41b85-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="41b85-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="41b85-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="41b85-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="41b85-110">Attributes and elements</span></span>

<span data-ttu-id="41b85-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41b85-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41b85-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="41b85-112">Attributes</span></span>

<span data-ttu-id="41b85-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41b85-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41b85-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41b85-114">Child elements</span></span>

<span data-ttu-id="41b85-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="41b85-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41b85-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41b85-116">Parent elements</span></span>

|<span data-ttu-id="41b85-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41b85-117">**Element**</span></span>|<span data-ttu-id="41b85-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41b85-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41b85-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="41b85-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="41b85-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="41b85-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41b85-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="41b85-121">Text value</span></span>

<span data-ttu-id="41b85-122">O valor de texto indica se o domínio é necessário para autenticação.</span><span class="sxs-lookup"><span data-stu-id="41b85-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="41b85-123">Os valores possíveis estão **ativados** e **desativados**.</span><span class="sxs-lookup"><span data-stu-id="41b85-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="41b85-124">Se o valor estiver **ativado**, a solicitação subsequente deverá conter o domínio da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="41b85-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41b85-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="41b85-125">Remarks</span></span>

<span data-ttu-id="41b85-126">Se o domínio não for especificado no elemento [LoginName (POX)](loginname-pox.md) ou se o elemento **LoginName** não tiver sido especificado, o usuário deverá inserir o domínio antes que a autenticação seja bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="41b85-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="41b85-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="41b85-127">See also</span></span>

- [<span data-ttu-id="41b85-128">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="41b85-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

