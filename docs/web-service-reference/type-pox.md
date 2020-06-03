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
description: O elemento Type identifica o tipo da conta de email configurada.
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465097"
---
# <a name="type-pox"></a><span data-ttu-id="621db-103">Tipo (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-103">Type (POX)</span></span>

<span data-ttu-id="621db-104">O elemento **Type** identifica o tipo da conta de email configurada.</span><span class="sxs-lookup"><span data-stu-id="621db-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="621db-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="621db-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="621db-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="621db-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="621db-109">Tipo (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="621db-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="621db-110">Attributes and elements</span></span>

<span data-ttu-id="621db-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="621db-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="621db-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="621db-112">Attributes</span></span>

<span data-ttu-id="621db-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="621db-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="621db-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="621db-114">Child elements</span></span>

<span data-ttu-id="621db-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="621db-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="621db-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="621db-116">Parent elements</span></span>

|<span data-ttu-id="621db-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="621db-117">**Element**</span></span>|<span data-ttu-id="621db-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="621db-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="621db-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="621db-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="621db-120">Contém as especificações para conectar um cliente ao servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="621db-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="621db-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="621db-121">Text value</span></span>

<span data-ttu-id="621db-122">O valor de texto representa o tipo de conta de email.</span><span class="sxs-lookup"><span data-stu-id="621db-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="621db-123">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="621db-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="621db-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="621db-124">**Value**</span></span>|<span data-ttu-id="621db-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="621db-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="621db-126">Exchange</span><span class="sxs-lookup"><span data-stu-id="621db-126">EXCH</span></span>  <br/> |<span data-ttu-id="621db-127">O protocolo usado para se conectar ao servidor é o RPC do Exchange.</span><span class="sxs-lookup"><span data-stu-id="621db-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="621db-128">Exhttp</span><span class="sxs-lookup"><span data-stu-id="621db-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="621db-129">O protocolo usado para estabelecer conexão com as conexões RPC/HTTP do servidor.</span><span class="sxs-lookup"><span data-stu-id="621db-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="621db-130">EXPR</span><span class="sxs-lookup"><span data-stu-id="621db-130">EXPR</span></span>  <br/> |<span data-ttu-id="621db-131">O protocolo usado para se conectar ao servidor é Exchange RPC sobre HTTP, usando um servidor proxy RPC.</span><span class="sxs-lookup"><span data-stu-id="621db-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="621db-132">Isso só é aplicável quando o elemento [AccountType (POX)](accounttype-pox.md) é definido como email.</span><span class="sxs-lookup"><span data-stu-id="621db-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="621db-133">WEB</span><span class="sxs-lookup"><span data-stu-id="621db-133">WEB</span></span>  <br/> |<span data-ttu-id="621db-134">O email é acessado a partir de um navegador da Web usando a URL especificada no elemento [servidor (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="621db-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="621db-135">Isso só é aplicável quando o elemento [AccountType (POX)](accounttype-pox.md) é definido como email.</span><span class="sxs-lookup"><span data-stu-id="621db-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="621db-136">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="621db-136">Version differences</span></span>

<span data-ttu-id="621db-137">O Office 365, o Exchange Online e as versões locais do Exchange começando com o Build 15.00.0995.014 retornam um valor de "exhttp" somente se o servidor estiver configurado para aceitar conexões RPC/HTTP e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "ExHttpInfo".</span><span class="sxs-lookup"><span data-stu-id="621db-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="621db-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="621db-138">See also</span></span>



[<span data-ttu-id="621db-139">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="621db-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

