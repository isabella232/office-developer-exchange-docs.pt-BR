---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: O elemento InternalUrl contém a URL para conectar um cliente ao servidor de catálogo de endereços ou à caixa de correio de um usuário de dentro da organização do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 9c6ba621a681ec54d88089de6b7ae1eefdebc679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465573"
---
# <a name="internalurl-pox"></a><span data-ttu-id="e1424-103">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e1424-103">InternalUrl (POX)</span></span>

<span data-ttu-id="e1424-104">O elemento **InternalURL** contém a URL para conectar um cliente ao servidor de catálogo de endereços ou à caixa de correio de um usuário de dentro da organização do usuário usando o protocolo MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="e1424-104">The **InternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from inside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e1424-105">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1424-105">Attributes and elements</span></span>

<span data-ttu-id="e1424-106">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1424-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1424-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1424-107">Attributes</span></span>

<span data-ttu-id="e1424-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1424-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1424-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1424-109">Child elements</span></span>

<span data-ttu-id="e1424-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1424-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1424-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1424-111">Parent elements</span></span>

|<span data-ttu-id="e1424-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1424-112">**Element**</span></span>|<span data-ttu-id="e1424-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1424-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1424-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="e1424-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="e1424-115">Contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e1424-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="e1424-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="e1424-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="e1424-117">Contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e1424-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1424-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e1424-118">Text value</span></span>

<span data-ttu-id="e1424-119">O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário de dentro da organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1424-119">The text value represents a URL that can be used to access an address book server or user's mailbox from inside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1424-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1424-120">Remarks</span></span>

<span data-ttu-id="e1424-121">O elemento **InternalURL** pode estar presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp".</span><span class="sxs-lookup"><span data-stu-id="e1424-121">The **InternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="e1424-122">O elemento **InternalURL** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="e1424-122">The **InternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e1424-123">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e1424-123">See also</span></span>



[<span data-ttu-id="e1424-124">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="e1424-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

