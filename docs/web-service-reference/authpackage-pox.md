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
description: O elemento AuthPackage Especifica o esquema de autenticação usado quando se autenticar no servidor do Exchange que possui a função de servidor de caixa de correio instalada.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751236"
---
# <a name="authpackage-pox"></a><span data-ttu-id="67058-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-103">AuthPackage (POX)</span></span>

<span data-ttu-id="67058-104">O elemento **AuthPackage** Especifica o esquema de autenticação usado quando se autenticar no servidor do Exchange que possui a função de servidor de caixa de correio instalada.</span><span class="sxs-lookup"><span data-stu-id="67058-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="67058-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="67058-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="67058-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="67058-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="67058-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="67058-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="67058-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="67058-110">Attributes and elements</span></span>

<span data-ttu-id="67058-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="67058-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67058-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="67058-112">Attributes</span></span>

<span data-ttu-id="67058-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="67058-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67058-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="67058-114">Child elements</span></span>

<span data-ttu-id="67058-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="67058-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67058-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="67058-116">Parent elements</span></span>

|<span data-ttu-id="67058-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67058-117">**Element**</span></span>|<span data-ttu-id="67058-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67058-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67058-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="67058-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="67058-120">Contém as especificações para conectar um cliente para o servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="67058-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67058-121">Text value</span><span class="sxs-lookup"><span data-stu-id="67058-121">Text value</span></span>

<span data-ttu-id="67058-122">O valor de texto Especifica o esquema de autenticação que é usado durante a autenticação com base no servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="67058-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="67058-123">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="67058-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="67058-124">básico</span><span class="sxs-lookup"><span data-stu-id="67058-124">basic</span></span>
- <span data-ttu-id="67058-125">KERBTRAY localizado</span><span class="sxs-lookup"><span data-stu-id="67058-125">kerb</span></span>
- <span data-ttu-id="67058-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="67058-126">kerbntlm</span></span>
- <span data-ttu-id="67058-127">NTLM</span><span class="sxs-lookup"><span data-stu-id="67058-127">ntlm</span></span>
- <span data-ttu-id="67058-128">certificado</span><span class="sxs-lookup"><span data-stu-id="67058-128">certificate</span></span>
- <span data-ttu-id="67058-129">negociar</span><span class="sxs-lookup"><span data-stu-id="67058-129">negotiate</span></span>
- <span data-ttu-id="67058-130">nego2</span><span class="sxs-lookup"><span data-stu-id="67058-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="67058-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="67058-131">Remarks</span></span>

<span data-ttu-id="67058-132">O elemento **AuthPackage** é usado apenas quando o elemento de [Tipo POX ()](type-pox.md) tem um valor de texto de EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="67058-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="67058-133">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="67058-133">Version differences</span></span>

<span data-ttu-id="67058-134">O Office 365, Exchange Online e versões de local do Exchange começando com compilação 15.00.0995.014 retorno um valor igual a "negociar" somente se o servidor está configurado para usar a autenticação negociar e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contém "Negociar".</span><span class="sxs-lookup"><span data-stu-id="67058-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="67058-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="67058-135">See also</span></span>

- [<span data-ttu-id="67058-136">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="67058-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

