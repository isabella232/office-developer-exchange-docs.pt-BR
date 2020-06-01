---
title: EcpUrl-publish (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: O elemento EcpUrl-Publish especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações de publicação de calendário para um usuário habilitado para email.
ms.openlocfilehash: 98cac9132c1ba6e368be6337fbf3b522a02cb47a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458002"
---
# <a name="ecpurl-publish-pox"></a><span data-ttu-id="ac3d2-103">EcpUrl-publish (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-103">EcpUrl-publish (POX)</span></span>

<span data-ttu-id="ac3d2-104">O elemento **EcpUrl-Publish** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de publicação de calendário para um usuário habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="ac3d2-104">The **EcpUrl-publish** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="ac3d2-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ac3d2-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ac3d2-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ac3d2-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ac3d2-109">EcpUrl-publish (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-109">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ac3d2-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ac3d2-110">Attributes and elements</span></span>

<span data-ttu-id="ac3d2-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac3d2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac3d2-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac3d2-112">Attributes</span></span>

<span data-ttu-id="ac3d2-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac3d2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac3d2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac3d2-114">Child elements</span></span>

<span data-ttu-id="ac3d2-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac3d2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac3d2-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac3d2-116">Parent elements</span></span>

|<span data-ttu-id="ac3d2-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac3d2-117">**Element**</span></span>|<span data-ttu-id="ac3d2-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac3d2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac3d2-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="ac3d2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ac3d2-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ac3d2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac3d2-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ac3d2-121">Text value</span></span>

<span data-ttu-id="ac3d2-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de publicação de calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac3d2-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac3d2-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac3d2-123">Remarks</span></span>

<span data-ttu-id="ac3d2-124">O elemento **EcpUrl-Publish** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="ac3d2-124">The **EcpUrl-publish** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ac3d2-125">Também consulte</span><span class="sxs-lookup"><span data-stu-id="ac3d2-125">See also</span></span>



[<span data-ttu-id="ac3d2-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="ac3d2-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

