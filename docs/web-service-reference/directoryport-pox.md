---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: O elemento DirectoryPort especifica a porta usada para se conectar ao diretório quando o protocolo NSPI (interface de provedor de serviço de nome) é usado.
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462084"
---
# <a name="directoryport-pox"></a><span data-ttu-id="5dcb4-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="5dcb4-104">O elemento **DirectoryPort** especifica a porta usada para se conectar ao diretório quando o protocolo NSPI (interface de provedor de serviço de nome) é usado.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="5dcb4-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="5dcb4-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="5dcb4-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="5dcb4-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="5dcb4-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5dcb4-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5dcb4-110">Attributes and elements</span></span>

<span data-ttu-id="5dcb4-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dcb4-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="5dcb4-112">Attributes</span></span>

<span data-ttu-id="5dcb4-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dcb4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dcb4-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5dcb4-114">Child elements</span></span>

<span data-ttu-id="5dcb4-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dcb4-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5dcb4-116">Parent elements</span></span>

|<span data-ttu-id="5dcb4-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5dcb4-117">**Element**</span></span>|<span data-ttu-id="5dcb4-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5dcb4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dcb4-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="5dcb4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="5dcb4-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5dcb4-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5dcb4-121">Text value</span></span>

<span data-ttu-id="5dcb4-122">O valor de texto representa a porta usada para acessar o servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dcb4-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="5dcb4-123">Remarks</span></span>

<span data-ttu-id="5dcb4-124">O elemento **DirectoryPort** é usado somente quando o elemento [tipo (POX)](type-pox.md) é igual a Exch ou expr.</span><span class="sxs-lookup"><span data-stu-id="5dcb4-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5dcb4-125">Também consulte</span><span class="sxs-lookup"><span data-stu-id="5dcb4-125">See also</span></span>

- [<span data-ttu-id="5dcb4-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="5dcb4-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

