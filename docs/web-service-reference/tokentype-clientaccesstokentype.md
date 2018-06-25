---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: O elemento TokenType identifica o tipo de token de acesso de cliente que será retornado na resposta GetClientAccessToken.
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837773"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="916ad-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="916ad-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="916ad-104">O elemento **TokenType** identifica o tipo de token de acesso de cliente que será retornado na resposta **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="916ad-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="916ad-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="916ad-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="916ad-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="916ad-106">Attributes and elements</span></span>

<span data-ttu-id="916ad-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="916ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="916ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="916ad-108">Attributes</span></span>

<span data-ttu-id="916ad-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="916ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="916ad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="916ad-110">Child elements</span></span>

<span data-ttu-id="916ad-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="916ad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="916ad-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="916ad-112">Parent elements</span></span>

<span data-ttu-id="916ad-113">[TokenRequest](tokenrequest.md) | [(ClientAccessTokenType) de Token](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="916ad-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="916ad-114">Text value</span><span class="sxs-lookup"><span data-stu-id="916ad-114">Text value</span></span>

<span data-ttu-id="916ad-115">Um valor de texto de **CallerIdentity** significa que um token de acesso de cliente de identidade de chamador será retornado.</span><span class="sxs-lookup"><span data-stu-id="916ad-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="916ad-116">Um valor de texto de **ExtensionCallback** indica que um token de acesso de cliente de retorno de chamada de extensão será retornado.</span><span class="sxs-lookup"><span data-stu-id="916ad-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="916ad-117">Um valor de texto de **ScopedToken** indica que o token de acesso do cliente é um token de escopo.</span><span class="sxs-lookup"><span data-stu-id="916ad-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="916ad-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="916ad-118">Remarks</span></span>

<span data-ttu-id="916ad-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="916ad-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="916ad-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="916ad-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="916ad-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="916ad-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="916ad-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="916ad-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="916ad-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="916ad-123">Schema name</span></span>  <br/> |<span data-ttu-id="916ad-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="916ad-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="916ad-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="916ad-125">Validation file</span></span>  <br/> |<span data-ttu-id="916ad-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="916ad-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="916ad-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="916ad-127">Can be empty</span></span>  <br/> |<span data-ttu-id="916ad-128">false</span><span class="sxs-lookup"><span data-stu-id="916ad-128">false</span></span>  <br/> |
   

