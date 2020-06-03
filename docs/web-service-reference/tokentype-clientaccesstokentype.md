---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: O elemento TokenType identifica o tipo de token de acesso para cliente que será retornado na resposta GetClientAccessToken.
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466049"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="80f4d-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="80f4d-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="80f4d-104">O elemento **TokenType** identifica o tipo de token de acesso para cliente que será retornado na resposta **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="80f4d-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="80f4d-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="80f4d-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80f4d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="80f4d-106">Attributes and elements</span></span>

<span data-ttu-id="80f4d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="80f4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80f4d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="80f4d-108">Attributes</span></span>

<span data-ttu-id="80f4d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80f4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80f4d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="80f4d-110">Child elements</span></span>

<span data-ttu-id="80f4d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="80f4d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80f4d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="80f4d-112">Parent elements</span></span>

<span data-ttu-id="80f4d-113">[TokenRequest](tokenrequest.md)  |  [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="80f4d-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="80f4d-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="80f4d-114">Text value</span></span>

<span data-ttu-id="80f4d-115">Um valor de texto **CallerIdentity** significa que um token de acesso para cliente de identidade do chamador é retornado.</span><span class="sxs-lookup"><span data-stu-id="80f4d-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="80f4d-116">Um valor de texto **ExtensionCallback** indica que um token de retorno de chamada de cliente de extensão é retornado.</span><span class="sxs-lookup"><span data-stu-id="80f4d-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="80f4d-117">Um valor de texto de **ScopedToken** indica que o token de acesso do cliente é um token de escopo.</span><span class="sxs-lookup"><span data-stu-id="80f4d-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80f4d-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="80f4d-118">Remarks</span></span>

<span data-ttu-id="80f4d-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="80f4d-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="80f4d-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80f4d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80f4d-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="80f4d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80f4d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="80f4d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80f4d-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="80f4d-123">Schema name</span></span>  <br/> |<span data-ttu-id="80f4d-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="80f4d-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="80f4d-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="80f4d-125">Validation file</span></span>  <br/> |<span data-ttu-id="80f4d-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="80f4d-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80f4d-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="80f4d-127">Can be empty</span></span>  <br/> |<span data-ttu-id="80f4d-128">falso</span><span class="sxs-lookup"><span data-stu-id="80f4d-128">false</span></span>  <br/> |
   

