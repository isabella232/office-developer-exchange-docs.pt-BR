---
title: EcpUrl-extinstall (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: f81807e6-93de-4e47-afee-1e1ae6a85054
description: O elemento EcpUrl-extinstall especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para exibir ou alterar os aplicativos de email instalados atualmente na caixa de correio do usuário.
ms.openlocfilehash: 889e0ca3bdcdce4b557fe066db2918fde4abaa9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461300"
---
# <a name="ecpurl-extinstall-pox"></a><span data-ttu-id="8d714-103">EcpUrl-extinstall (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-103">EcpUrl-extinstall (POX)</span></span>

<span data-ttu-id="8d714-104">O elemento **EcpUrl-extinstall** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para exibir ou alterar os aplicativos de email instalados atualmente na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d714-104">The **EcpUrl-extinstall** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change the mail apps currently installed in the user's mailbox.</span></span> 
  
[<span data-ttu-id="8d714-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8d714-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8d714-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8d714-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8d714-109">EcpUrl-extinstall (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-109">EcpUrl-extinstall (POX)</span></span>](ecpurl-extinstall-pox.md)
  
```XML
<EcpUrl-extinstall/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8d714-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8d714-110">Attributes and elements</span></span>

<span data-ttu-id="8d714-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d714-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d714-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d714-112">Attributes</span></span>

<span data-ttu-id="8d714-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d714-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d714-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d714-114">Child elements</span></span>

<span data-ttu-id="8d714-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d714-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d714-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d714-116">Parent elements</span></span>

|<span data-ttu-id="8d714-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d714-117">**Element**</span></span>|<span data-ttu-id="8d714-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d714-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d714-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8d714-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8d714-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8d714-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d714-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8d714-121">Text value</span></span>

<span data-ttu-id="8d714-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email atualmente instalados na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d714-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change the mail apps currently installed in the user's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8d714-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d714-123">Remarks</span></span>

<span data-ttu-id="8d714-124">O elemento **EcpUrl-extinstall** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="8d714-124">The **EcpUrl-extinstall** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8d714-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d714-125">See also</span></span>



[<span data-ttu-id="8d714-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="8d714-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

