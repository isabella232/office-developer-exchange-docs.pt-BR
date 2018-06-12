---
title: Externo (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: O elemento externo contém uma coleção de URLs que um cliente pode usar para se conectar ao Exchange de fora da rede da organização.
ms.openlocfilehash: 7f01fc29b5ce63b02de0a4a6e42887dcffbb4b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752184"
---
# <a name="external-pox"></a><span data-ttu-id="119c1-103">Externo (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-103">External (POX)</span></span>

<span data-ttu-id="119c1-104">O elemento **externo** contém uma coleção de URLs que um cliente pode usar para se conectar ao Exchange de fora da rede da organização.</span><span class="sxs-lookup"><span data-stu-id="119c1-104">The **External** element contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span> 
  
[<span data-ttu-id="119c1-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="119c1-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="119c1-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="119c1-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="119c1-109">Externo (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-109">External (POX)</span></span>](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="119c1-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="119c1-110">Attributes and elements</span></span>

<span data-ttu-id="119c1-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="119c1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="119c1-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="119c1-112">Attributes</span></span>

<span data-ttu-id="119c1-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="119c1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="119c1-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="119c1-114">Child elements</span></span>

|<span data-ttu-id="119c1-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="119c1-115">**Element**</span></span>|<span data-ttu-id="119c1-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="119c1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="119c1-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="119c1-118">Descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server que possui a função acesso para cliente instalada que hospeda o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="119c1-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="119c1-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="119c1-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="119c1-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="119c1-121">Esse elemento de **protocolo** possui apenas dois elementos filho: um elemento de [Tipo (POX)](type-pox.md) especificar o protocolo de conexão e um elemento [ASUrl POX ()](asurl-pox.md) , especificando o ponto de extremidade do EWS para o serviço web de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="119c1-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="119c1-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="119c1-122">Parent elements</span></span>

|<span data-ttu-id="119c1-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="119c1-123">**Element**</span></span>|<span data-ttu-id="119c1-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="119c1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="119c1-125">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="119c1-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="119c1-126">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="119c1-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="119c1-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="119c1-127">Remarks</span></span>

<span data-ttu-id="119c1-128">O **externo** é um elemento filho opcionais do elemento de **protocolo** .</span><span class="sxs-lookup"><span data-stu-id="119c1-128">The **External** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="119c1-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="119c1-129">See also</span></span>



[<span data-ttu-id="119c1-130">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="119c1-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

