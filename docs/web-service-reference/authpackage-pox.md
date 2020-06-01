---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: O elemento AuthPackage especifica o esquema de autenticação que é usado na autenticação no servidor do Exchange que tem a função de servidor caixa de Correio instalada.
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459101"
---
# <a name="authpackage-pox"></a><span data-ttu-id="195a5-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-103">AuthPackage (POX)</span></span>

<span data-ttu-id="195a5-104">O elemento **AuthPackage** especifica o esquema de autenticação que é usado na autenticação no servidor do Exchange que tem a função de servidor caixa de Correio instalada.</span><span class="sxs-lookup"><span data-stu-id="195a5-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="195a5-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="195a5-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="195a5-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="195a5-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="195a5-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="195a5-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="195a5-110">Attributes and elements</span></span>

<span data-ttu-id="195a5-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="195a5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="195a5-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="195a5-112">Attributes</span></span>

<span data-ttu-id="195a5-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="195a5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="195a5-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="195a5-114">Child elements</span></span>

<span data-ttu-id="195a5-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="195a5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="195a5-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="195a5-116">Parent elements</span></span>

|<span data-ttu-id="195a5-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="195a5-117">**Element**</span></span>|<span data-ttu-id="195a5-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="195a5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="195a5-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="195a5-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="195a5-120">Contém as especificações para conectar um cliente ao servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="195a5-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="195a5-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="195a5-121">Text value</span></span>

<span data-ttu-id="195a5-122">O valor de texto especifica o esquema de autenticação usado na autenticação no servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="195a5-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="195a5-123">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="195a5-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="195a5-124">Basic</span><span class="sxs-lookup"><span data-stu-id="195a5-124">basic</span></span>
- <span data-ttu-id="195a5-125">kerb</span><span class="sxs-lookup"><span data-stu-id="195a5-125">kerb</span></span>
- <span data-ttu-id="195a5-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="195a5-126">kerbntlm</span></span>
- <span data-ttu-id="195a5-127">NTML</span><span class="sxs-lookup"><span data-stu-id="195a5-127">ntlm</span></span>
- <span data-ttu-id="195a5-128">certificado</span><span class="sxs-lookup"><span data-stu-id="195a5-128">certificate</span></span>
- <span data-ttu-id="195a5-129">negocia</span><span class="sxs-lookup"><span data-stu-id="195a5-129">negotiate</span></span>
- <span data-ttu-id="195a5-130">nego2</span><span class="sxs-lookup"><span data-stu-id="195a5-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="195a5-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="195a5-131">Remarks</span></span>

<span data-ttu-id="195a5-132">O elemento **AuthPackage** é usado somente quando o elemento [tipo (POX)](type-pox.md) tem um valor de texto de Exch ou expr.</span><span class="sxs-lookup"><span data-stu-id="195a5-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="195a5-133">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="195a5-133">Version differences</span></span>

<span data-ttu-id="195a5-134">O Office 365, o Exchange Online e as versões locais do Exchange começando com o Build 15.00.0995.014 retornam um valor de "Negotiate" somente se o servidor estiver configurado para usar a autenticação de negociação e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "negociar".</span><span class="sxs-lookup"><span data-stu-id="195a5-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="195a5-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="195a5-135">See also</span></span>

- [<span data-ttu-id="195a5-136">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="195a5-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

