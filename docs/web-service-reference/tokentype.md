---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: O elemento TokenType Especifica o tipo de token.
ms.openlocfilehash: 5c8e880f035ed74776a7c77e4b4e60ca46d66d4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837767"
---
# <a name="tokentype"></a><span data-ttu-id="3c5cd-103">TokenType</span><span class="sxs-lookup"><span data-stu-id="3c5cd-103">TokenType</span></span>

<span data-ttu-id="3c5cd-104">O elemento **TokenType** Especifica o tipo de token.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="3c5cd-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="3c5cd-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c5cd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3c5cd-106">Attributes and elements</span></span>

<span data-ttu-id="3c5cd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c5cd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c5cd-108">Attributes</span></span>

<span data-ttu-id="3c5cd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c5cd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c5cd-110">Child elements</span></span>

<span data-ttu-id="3c5cd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c5cd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c5cd-112">Parent elements</span></span>

<span data-ttu-id="3c5cd-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span><span class="sxs-lookup"><span data-stu-id="3c5cd-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3c5cd-114">Text value</span><span class="sxs-lookup"><span data-stu-id="3c5cd-114">Text value</span></span>

<span data-ttu-id="3c5cd-115">O valor de texto do elemento **TokenType** é o tipo de token.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="3c5cd-116">O valor de texto da **CallerIdentity** indica que o token é um token de identidade do chamador.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="3c5cd-117">O valor de texto da **ExtensionCallback** indica que o token é para um retorno de chamada de extensão.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="3c5cd-118">O valor de texto da **ScopedToken** indica que o token de acesso do cliente é um token de escopo.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c5cd-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="3c5cd-119">Remarks</span></span>

<span data-ttu-id="3c5cd-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3c5cd-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c5cd-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c5cd-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3c5cd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c5cd-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c5cd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c5cd-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c5cd-124">Schema name</span></span>  <br/> |<span data-ttu-id="3c5cd-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3c5cd-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c5cd-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c5cd-126">Validation file</span></span>  <br/> |<span data-ttu-id="3c5cd-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c5cd-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c5cd-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3c5cd-128">Can be empty</span></span>  <br/> |<span data-ttu-id="3c5cd-129">false</span><span class="sxs-lookup"><span data-stu-id="3c5cd-129">false</span></span>  <br/> |
   

