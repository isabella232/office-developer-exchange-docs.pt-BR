---
title: Tipo (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: O elemento de tipo identifica o tipo da conta de email configurada.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837807"
---
# <a name="type-pox"></a><span data-ttu-id="1a45a-103">Tipo (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-103">Type (POX)</span></span>

<span data-ttu-id="1a45a-104">O **tipo** de elemento identifica o tipo da conta de email configurada.</span><span class="sxs-lookup"><span data-stu-id="1a45a-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="1a45a-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1a45a-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1a45a-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1a45a-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="1a45a-109">Tipo (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1a45a-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1a45a-110">Attributes and elements</span></span>

<span data-ttu-id="1a45a-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1a45a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a45a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="1a45a-112">Attributes</span></span>

<span data-ttu-id="1a45a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1a45a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a45a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1a45a-114">Child elements</span></span>

<span data-ttu-id="1a45a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1a45a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a45a-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1a45a-116">Parent elements</span></span>

|<span data-ttu-id="1a45a-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a45a-117">**Element**</span></span>|<span data-ttu-id="1a45a-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a45a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a45a-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="1a45a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1a45a-120">Contém as especificações para conectar um cliente para o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1a45a-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a45a-121">Text value</span><span class="sxs-lookup"><span data-stu-id="1a45a-121">Text value</span></span>

<span data-ttu-id="1a45a-122">O valor de texto representa o tipo de conta de email.</span><span class="sxs-lookup"><span data-stu-id="1a45a-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="1a45a-123">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="1a45a-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="1a45a-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="1a45a-124">**Value**</span></span>|<span data-ttu-id="1a45a-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a45a-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a45a-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="1a45a-126">EXCH</span></span>  <br/> |<span data-ttu-id="1a45a-127">O protocolo usado para conectar ao servidor é RPC do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a45a-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="1a45a-128">EXHTTP</span><span class="sxs-lookup"><span data-stu-id="1a45a-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="1a45a-129">O protocolo que é usado para conectar-se para as conexões de servidor RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1a45a-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="1a45a-130">EXPR</span><span class="sxs-lookup"><span data-stu-id="1a45a-130">EXPR</span></span>  <br/> |<span data-ttu-id="1a45a-131">O protocolo que é usado para conectar ao servidor é Exchange RPC sobre HTTP, usando um servidor proxy RPC.</span><span class="sxs-lookup"><span data-stu-id="1a45a-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="1a45a-132">Isso só é aplicável quando o elemento [AccountType POX ()](accounttype-pox.md) é definido como email.</span><span class="sxs-lookup"><span data-stu-id="1a45a-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="1a45a-133">WEB</span><span class="sxs-lookup"><span data-stu-id="1a45a-133">WEB</span></span>  <br/> |<span data-ttu-id="1a45a-134">Email é acessada a partir de um navegador da Web usando a URL especificada no elemento [Server POX ()](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="1a45a-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="1a45a-135">Isso só é aplicável quando o elemento [AccountType POX ()](accounttype-pox.md) é definido como email.</span><span class="sxs-lookup"><span data-stu-id="1a45a-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="1a45a-136">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="1a45a-136">Version differences</span></span>

<span data-ttu-id="1a45a-137">O Office 365, Exchange Online e versões de local do Exchange começando com compilação 15.00.0995.014 retorno um valor igual a "EXHTTP" somente se o servidor está configurado para aceitar conexões de RPC/HTTP e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contém "ExHttpInfo".</span><span class="sxs-lookup"><span data-stu-id="1a45a-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1a45a-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a45a-138">See also</span></span>



[<span data-ttu-id="1a45a-139">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="1a45a-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

