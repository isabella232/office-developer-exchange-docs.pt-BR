---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: O elemento EcpUrl-tmHiding especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site.
ms.openlocfilehash: 68b949db8b8d98caddbac3b9f96c5d5e55b104b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463528"
---
# <a name="ecpurl-tmhiding-pox"></a><span data-ttu-id="b9382-103">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-103">EcpUrl-tmHiding (POX)</span></span>

<span data-ttu-id="b9382-104">O elemento **EcpUrl-tmHiding** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="b9382-104">The **EcpUrl-tmHiding** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> 
  
[<span data-ttu-id="b9382-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="b9382-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="b9382-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="b9382-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="b9382-109">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-109">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b9382-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b9382-110">Attributes and elements</span></span>

<span data-ttu-id="b9382-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9382-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9382-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9382-112">Attributes</span></span>

<span data-ttu-id="b9382-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9382-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9382-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9382-114">Child elements</span></span>

<span data-ttu-id="b9382-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9382-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9382-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9382-116">Parent elements</span></span>

|<span data-ttu-id="b9382-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9382-117">**Element**</span></span>|<span data-ttu-id="b9382-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9382-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9382-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="b9382-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b9382-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b9382-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9382-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b9382-121">Text value</span></span>

<span data-ttu-id="b9382-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="b9382-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> <span data-ttu-id="b9382-123">O valor do elemento **EcpUrl-tmHiding** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b9382-123">The value of the **EcpUrl-tmHiding** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="b9382-124">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="b9382-124">**Parameter**</span></span>|<span data-ttu-id="b9382-125">**Substituir por**</span><span class="sxs-lookup"><span data-stu-id="b9382-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="b9382-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="b9382-126">_Id_</span></span> <br/> |<span data-ttu-id="b9382-127">O endereço de email SMTP ou o nome distinto do X500 da caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="b9382-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b9382-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="b9382-128">Remarks</span></span>

<span data-ttu-id="b9382-129">O elemento **EcpUrl-tmHiding** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="b9382-129">The **EcpUrl-tmHiding** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b9382-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b9382-130">See also</span></span>



[<span data-ttu-id="b9382-131">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="b9382-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

