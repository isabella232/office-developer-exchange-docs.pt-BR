---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: O elemento EcpUrl-tmHiding Especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl POX () para gerar uma URL que pode ser usada para cancelar o usuário a partir de uma caixa de correio do site.
ms.openlocfilehash: 461e9780dbd657ba0ba8b9ce9ea4fe902cba9698
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751958"
---
# <a name="ecpurl-tmhiding-pox"></a><span data-ttu-id="89dbf-103">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-103">EcpUrl-tmHiding (POX)</span></span>

<span data-ttu-id="89dbf-104">O elemento **EcpUrl-tmHiding** Especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para cancelar o usuário a partir de uma caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="89dbf-104">The **EcpUrl-tmHiding** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> 
  
[<span data-ttu-id="89dbf-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="89dbf-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="89dbf-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="89dbf-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="89dbf-109">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-109">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="89dbf-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="89dbf-110">Attributes and elements</span></span>

<span data-ttu-id="89dbf-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89dbf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89dbf-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="89dbf-112">Attributes</span></span>

<span data-ttu-id="89dbf-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89dbf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89dbf-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89dbf-114">Child elements</span></span>

<span data-ttu-id="89dbf-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89dbf-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89dbf-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89dbf-116">Parent elements</span></span>

|<span data-ttu-id="89dbf-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89dbf-117">**Element**</span></span>|<span data-ttu-id="89dbf-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89dbf-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89dbf-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="89dbf-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="89dbf-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="89dbf-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89dbf-121">Text value</span><span class="sxs-lookup"><span data-stu-id="89dbf-121">Text value</span></span>

<span data-ttu-id="89dbf-122">O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl POX ()](ecpurl-pox.md) para gerar uma URL que pode ser usada para cancelar o usuário a partir de uma caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="89dbf-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> <span data-ttu-id="89dbf-123">O valor do elemento **EcpUrl-tmHiding** contém parâmetros contidos ' <' e ' >' caracteres que são substituídas pelo cliente, conforme mostrado na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="89dbf-123">The value of the **EcpUrl-tmHiding** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="89dbf-124">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="89dbf-124">**Parameter**</span></span>|<span data-ttu-id="89dbf-125">**Substituir com**</span><span class="sxs-lookup"><span data-stu-id="89dbf-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="89dbf-126">
  _Id_</span><span class="sxs-lookup"><span data-stu-id="89dbf-126">_Id_</span></span> <br/> |<span data-ttu-id="89dbf-127">O endereço de email SMTP ou o X500 diferenciados nome da caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="89dbf-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89dbf-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="89dbf-128">Remarks</span></span>

<span data-ttu-id="89dbf-129">O **EcpUrl-tmHiding** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="89dbf-129">The **EcpUrl-tmHiding** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="89dbf-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="89dbf-130">See also</span></span>



[<span data-ttu-id="89dbf-131">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="89dbf-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

