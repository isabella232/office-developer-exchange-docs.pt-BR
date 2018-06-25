---
title: Interno (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: O elemento interno contém a coleção de URLs que um cliente pode usar para se conectar ao Exchange de dentro da rede da organização.
ms.openlocfilehash: 0dc5b679af98b52f15ef3b40181c2d97f102f373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823946"
---
# <a name="internal-pox"></a><span data-ttu-id="9b4f2-103">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-103">Internal (POX)</span></span>

<span data-ttu-id="9b4f2-104">O elemento de **Internal** contém a coleção de URLs que um cliente pode usar para se conectar ao Exchange de dentro da rede da organização.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="9b4f2-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9b4f2-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9b4f2-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9b4f2-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9b4f2-109">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9b4f2-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9b4f2-110">Attributes and elements</span></span>

<span data-ttu-id="9b4f2-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b4f2-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="9b4f2-112">Attributes</span></span>

<span data-ttu-id="9b4f2-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b4f2-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9b4f2-114">Child elements</span></span>

|<span data-ttu-id="9b4f2-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b4f2-115">**Element**</span></span>|<span data-ttu-id="9b4f2-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b4f2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b4f2-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="9b4f2-118">Descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server que possui a função acesso para cliente instalada que hospeda o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="9b4f2-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9b4f2-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="9b4f2-121">Esse elemento de **protocolo** possui apenas dois elementos filho: um elemento de [Tipo (POX)](type-pox.md) especificar o protocolo de conexão e um elemento [ASUrl POX ()](asurl-pox.md) , especificando o ponto de extremidade do EWS para o serviço web de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b4f2-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9b4f2-122">Parent elements</span></span>

|<span data-ttu-id="9b4f2-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b4f2-123">**Element**</span></span>|<span data-ttu-id="9b4f2-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b4f2-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b4f2-125">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9b4f2-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9b4f2-126">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9b4f2-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b4f2-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b4f2-127">Remarks</span></span>

<span data-ttu-id="9b4f2-128">O **interno** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="9b4f2-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9b4f2-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9b4f2-129">See also</span></span>



[<span data-ttu-id="9b4f2-130">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="9b4f2-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

