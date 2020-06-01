---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: O elemento AddressBook contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463633"
---
# <a name="addressbook-pox"></a><span data-ttu-id="15c77-103">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-103">AddressBook (POX)</span></span>

<span data-ttu-id="15c77-104">O elemento **AddressBook** contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="15c77-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="15c77-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="15c77-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="15c77-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="15c77-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="15c77-109">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="15c77-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="15c77-110">Attributes and elements</span></span>

<span data-ttu-id="15c77-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="15c77-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15c77-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="15c77-112">Attributes</span></span>

<span data-ttu-id="15c77-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15c77-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15c77-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="15c77-114">Child elements</span></span>

|<span data-ttu-id="15c77-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15c77-115">**Element**</span></span>|<span data-ttu-id="15c77-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15c77-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15c77-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="15c77-118">Contém a URL que deve ser usada para acessar o catálogo de endereços de fora da rede da organização usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="15c77-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="15c77-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="15c77-120">Contém a URL que deve ser usada para acessar o catálogo de endereços de dentro da rede da organização usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="15c77-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15c77-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="15c77-121">Parent elements</span></span>

|<span data-ttu-id="15c77-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15c77-122">**Element**</span></span>|<span data-ttu-id="15c77-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15c77-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15c77-124">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="15c77-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="15c77-125">Contém as especificações para conectar um cliente ao servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="15c77-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15c77-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="15c77-126">Remarks</span></span>

<span data-ttu-id="15c77-127">O elemento **AddressBook** está presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp".</span><span class="sxs-lookup"><span data-stu-id="15c77-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="15c77-128">O elemento **AddressBook** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="15c77-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="15c77-129">Também consulte</span><span class="sxs-lookup"><span data-stu-id="15c77-129">See also</span></span>

- [<span data-ttu-id="15c77-130">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="15c77-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

