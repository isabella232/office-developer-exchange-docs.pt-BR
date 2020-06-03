---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: O elemento ExternalUrl contém a URL para conectar um cliente ao servidor de catálogo de endereços ou caixa de correio de um usuário de fora da organização do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 94265051be68ed06d1dab8d46dd4ce29d8694c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457953"
---
# <a name="externalurl-pox"></a><span data-ttu-id="0b98b-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="0b98b-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="0b98b-104">O elemento **ExternalURL** contém a URL para conectar um cliente ao servidor de catálogo de endereços ou caixa de correio de um usuário de fora da organização do usuário usando o protocolo MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="0b98b-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0b98b-105">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0b98b-105">Attributes and elements</span></span>

<span data-ttu-id="0b98b-106">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b98b-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b98b-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b98b-107">Attributes</span></span>

<span data-ttu-id="0b98b-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b98b-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b98b-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b98b-109">Child elements</span></span>

<span data-ttu-id="0b98b-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b98b-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b98b-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b98b-111">Parent elements</span></span>

|<span data-ttu-id="0b98b-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b98b-112">**Element**</span></span>|<span data-ttu-id="0b98b-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b98b-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b98b-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="0b98b-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="0b98b-115">Contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="0b98b-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="0b98b-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="0b98b-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="0b98b-117">Contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="0b98b-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b98b-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0b98b-118">Text value</span></span>

<span data-ttu-id="0b98b-119">O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="0b98b-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b98b-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b98b-120">Remarks</span></span>

<span data-ttu-id="0b98b-121">O elemento **ExternalURL** pode estar presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp".</span><span class="sxs-lookup"><span data-stu-id="0b98b-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="0b98b-122">O elemento **ExternalURL** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="0b98b-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0b98b-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="0b98b-123">See also</span></span>



[<span data-ttu-id="0b98b-124">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="0b98b-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

