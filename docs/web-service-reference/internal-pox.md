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
description: O elemento Internal contém a coleção de URLs que um cliente pode usar para se conectar ao Exchange de dentro da rede da organização.
ms.openlocfilehash: 8164a018a11f9bae9c3abcbfebf6cf0694ca4183
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465594"
---
# <a name="internal-pox"></a><span data-ttu-id="c2b70-103">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-103">Internal (POX)</span></span>

<span data-ttu-id="c2b70-104">O elemento **Internal** contém a coleção de URLs que um cliente pode usar para se conectar ao Exchange de dentro da rede da organização.</span><span class="sxs-lookup"><span data-stu-id="c2b70-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="c2b70-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c2b70-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c2b70-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c2b70-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="c2b70-109">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c2b70-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c2b70-110">Attributes and elements</span></span>

<span data-ttu-id="c2b70-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2b70-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2b70-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2b70-112">Attributes</span></span>

<span data-ttu-id="c2b70-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2b70-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2b70-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2b70-114">Child elements</span></span>

|<span data-ttu-id="c2b70-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2b70-115">**Element**</span></span>|<span data-ttu-id="c2b70-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2b70-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2b70-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="c2b70-118">Descreve a URL e o esquema de autenticação que é usado para acessar um determinado computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada que hospeda o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="c2b70-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="c2b70-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c2b70-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c2b70-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="c2b70-121">Este elemento de **protocolo** tem apenas dois elementos filho: um [tipo (POX)](type-pox.md) que especifica o protocolo de conexão e um elemento [ASUrl (POX)](asurl-pox.md) , ESPECIFICANDO o ponto de extremidade do EWS para o serviço Web de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2b70-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2b70-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2b70-122">Parent elements</span></span>

|<span data-ttu-id="c2b70-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2b70-123">**Element**</span></span>|<span data-ttu-id="c2b70-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2b70-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2b70-125">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c2b70-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c2b70-126">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c2b70-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2b70-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2b70-127">Remarks</span></span>

<span data-ttu-id="c2b70-128">O elemento **Internal** é um elemento filho opcional do elemento **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="c2b70-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c2b70-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="c2b70-129">See also</span></span>



[<span data-ttu-id="c2b70-130">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="c2b70-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

