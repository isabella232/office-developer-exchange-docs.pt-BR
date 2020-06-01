---
title: EcpUrl-TM (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: O elemento EcpUrl-TM especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar uma lista de todas as caixas de correio de site das quais um usuário habilitado para email é membro no momento.
ms.openlocfilehash: 8d4c787e2eeae5300cd0496f199ea71baace98ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463542"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="40146-103">EcpUrl-TM (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="40146-104">O elemento **EcpUrl-TM** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar uma lista de todas as caixas de correio de site das quais um usuário habilitado para email é membro no momento.</span><span class="sxs-lookup"><span data-stu-id="40146-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="40146-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="40146-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="40146-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="40146-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="40146-109">EcpUrl-TM (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="40146-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="40146-110">Attributes and elements</span></span>

<span data-ttu-id="40146-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40146-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40146-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="40146-112">Attributes</span></span>

<span data-ttu-id="40146-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40146-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40146-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40146-114">Child elements</span></span>

<span data-ttu-id="40146-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="40146-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40146-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40146-116">Parent elements</span></span>

|<span data-ttu-id="40146-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40146-117">**Element**</span></span>|<span data-ttu-id="40146-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40146-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40146-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="40146-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="40146-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="40146-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40146-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="40146-121">Text value</span></span>

<span data-ttu-id="40146-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de caixas de correio de site para o usuário.</span><span class="sxs-lookup"><span data-stu-id="40146-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="40146-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="40146-123">Remarks</span></span>

<span data-ttu-id="40146-124">O elemento **EcpUrl-TM** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="40146-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="40146-125">Também consulte</span><span class="sxs-lookup"><span data-stu-id="40146-125">See also</span></span>



[<span data-ttu-id="40146-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="40146-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

