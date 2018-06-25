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
description: O elemento DirectoryPort Especifica a porta usada para conectar ao diretório quando o protocolo de Interface de provedor de serviço de nome (NSPI) é usado.
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751819"
---
# <a name="directoryport-pox"></a><span data-ttu-id="fdde3-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="fdde3-104">O elemento **DirectoryPort** Especifica a porta usada para conectar ao diretório quando o protocolo de Interface de provedor de serviço de nome (NSPI) é usado.</span><span class="sxs-lookup"><span data-stu-id="fdde3-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="fdde3-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="fdde3-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="fdde3-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="fdde3-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="fdde3-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="fdde3-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fdde3-110">Attributes and elements</span></span>

<span data-ttu-id="fdde3-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fdde3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdde3-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="fdde3-112">Attributes</span></span>

<span data-ttu-id="fdde3-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fdde3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdde3-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fdde3-114">Child elements</span></span>

<span data-ttu-id="fdde3-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fdde3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdde3-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fdde3-116">Parent elements</span></span>

|<span data-ttu-id="fdde3-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fdde3-117">**Element**</span></span>|<span data-ttu-id="fdde3-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fdde3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdde3-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="fdde3-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="fdde3-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="fdde3-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fdde3-121">Text value</span><span class="sxs-lookup"><span data-stu-id="fdde3-121">Text value</span></span>

<span data-ttu-id="fdde3-122">O valor de texto representa a porta usada para acessar o servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdde3-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdde3-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="fdde3-123">Remarks</span></span>

<span data-ttu-id="fdde3-124">O elemento **DirectoryPort** é usado apenas quando o elemento de [Tipo POX ()](type-pox.md) é igual a EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="fdde3-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fdde3-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="fdde3-125">See also</span></span>

- [<span data-ttu-id="fdde3-126">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="fdde3-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

