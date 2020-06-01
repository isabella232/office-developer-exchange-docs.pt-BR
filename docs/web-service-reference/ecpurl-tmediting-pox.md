---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: O elemento EcpUrl-tmEditing especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente.
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463535"
---
# <a name="ecpurl-tmediting-pox"></a><span data-ttu-id="416f5-103">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-103">EcpUrl-tmEditing (POX)</span></span>

<span data-ttu-id="416f5-104">O elemento **EcpUrl-tmEditing** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente.</span><span class="sxs-lookup"><span data-stu-id="416f5-104">The **EcpUrl-tmEditing** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> 
  
[<span data-ttu-id="416f5-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="416f5-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="416f5-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="416f5-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="416f5-109">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-109">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="416f5-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="416f5-110">Attributes and elements</span></span>

<span data-ttu-id="416f5-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="416f5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="416f5-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="416f5-112">Attributes</span></span>

<span data-ttu-id="416f5-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="416f5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="416f5-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="416f5-114">Child elements</span></span>

<span data-ttu-id="416f5-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="416f5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="416f5-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="416f5-116">Parent elements</span></span>

|<span data-ttu-id="416f5-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="416f5-117">**Element**</span></span>|<span data-ttu-id="416f5-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="416f5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="416f5-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="416f5-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="416f5-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="416f5-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="416f5-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="416f5-121">Text value</span></span>

<span data-ttu-id="416f5-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente.</span><span class="sxs-lookup"><span data-stu-id="416f5-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> <span data-ttu-id="416f5-123">O valor do elemento **EcpUrl-tmEditing** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="416f5-123">The value of the **EcpUrl-tmEditing** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="416f5-124">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="416f5-124">**Parameter**</span></span>|<span data-ttu-id="416f5-125">**Substituir por**</span><span class="sxs-lookup"><span data-stu-id="416f5-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="416f5-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="416f5-126">_Id_</span></span> <br/> |<span data-ttu-id="416f5-127">O endereço de email SMTP ou o nome distinto do X500 da caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="416f5-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="416f5-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="416f5-128">Remarks</span></span>

<span data-ttu-id="416f5-129">O elemento **EcpUrl-tmEditing** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="416f5-129">The **EcpUrl-tmEditing** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="416f5-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="416f5-130">See also</span></span>



[<span data-ttu-id="416f5-131">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="416f5-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

