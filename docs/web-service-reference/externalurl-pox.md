---
title: ExternalUrl POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: O elemento ExternalUrl contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário por meio do protocolo MAPI/HTTP.
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752222"
---
# <a name="externalurl-pox"></a><span data-ttu-id="633dc-103">ExternalUrl POX)</span><span class="sxs-lookup"><span data-stu-id="633dc-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="633dc-104">O elemento **ExternalUrl** contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário por meio do protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="633dc-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="633dc-105">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="633dc-105">Attributes and elements</span></span>

<span data-ttu-id="633dc-106">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="633dc-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="633dc-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="633dc-107">Attributes</span></span>

<span data-ttu-id="633dc-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="633dc-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="633dc-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="633dc-109">Child elements</span></span>

<span data-ttu-id="633dc-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="633dc-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="633dc-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="633dc-111">Parent elements</span></span>

|<span data-ttu-id="633dc-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="633dc-112">**Element**</span></span>|<span data-ttu-id="633dc-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="633dc-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="633dc-114">AddressBook POX)</span><span class="sxs-lookup"><span data-stu-id="633dc-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="633dc-115">Contém as especificações para conectar-se um cliente para o servidor de catálogo de endereços usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="633dc-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="633dc-116">Armazenamento_de_email (POX)</span><span class="sxs-lookup"><span data-stu-id="633dc-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="633dc-117">Contém as especificações para conectar um cliente de caixa de correio do usuário por meio do protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="633dc-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="633dc-118">Text value</span><span class="sxs-lookup"><span data-stu-id="633dc-118">Text value</span></span>

<span data-ttu-id="633dc-119">O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="633dc-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="633dc-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="633dc-120">Remarks</span></span>

<span data-ttu-id="633dc-121">O elemento **ExternalUrl** pode estar presente em uma resposta que tem um elemento de [Protocolo POX ()](protocol-pox.md) com um valor do atributo de **tipo** de "mapiHttp".</span><span class="sxs-lookup"><span data-stu-id="633dc-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="633dc-122">O elemento **ExternalUrl** está disponível para clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, e versões de local do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1) .</span><span class="sxs-lookup"><span data-stu-id="633dc-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="633dc-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="633dc-123">See also</span></span>



[<span data-ttu-id="633dc-124">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="633dc-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

