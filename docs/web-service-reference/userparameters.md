---
title: Parâmetros_do_usuário
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: O elemento Parâmetros_do_usuário contém uma lista de extensões de cliente habilitados e desabilitados.
ms.openlocfilehash: e0a72fe13255380ee56b32c863fb3bffb2e1ac5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837994"
---
# <a name="userparameters"></a><span data-ttu-id="40e4c-103">Parâmetros_do_usuário</span><span class="sxs-lookup"><span data-stu-id="40e4c-103">UserParameters</span></span>

<span data-ttu-id="40e4c-104">O elemento **Parâmetros_do_usuário** contém uma lista de extensões de cliente habilitados e desabilitados.</span><span class="sxs-lookup"><span data-stu-id="40e4c-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="40e4c-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="40e4c-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40e4c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="40e4c-106">Attributes and elements</span></span>

<span data-ttu-id="40e4c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40e4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40e4c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="40e4c-108">Attributes</span></span>

|<span data-ttu-id="40e4c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="40e4c-109">**Attribute**</span></span>|<span data-ttu-id="40e4c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40e4c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="40e4c-111">UserId</span><span class="sxs-lookup"><span data-stu-id="40e4c-111">UserId</span></span>  <br/> |<span data-ttu-id="40e4c-112">O valor de texto do atributo **UserId** é o identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="40e4c-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="40e4c-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="40e4c-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="40e4c-114">O valor de texto do **EnabledOnly** indica se a resposta contém apenas as extensões habilitadas.</span><span class="sxs-lookup"><span data-stu-id="40e4c-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="40e4c-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40e4c-115">Child elements</span></span>

<span data-ttu-id="40e4c-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="40e4c-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40e4c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40e4c-117">Parent elements</span></span>

[<span data-ttu-id="40e4c-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="40e4c-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="40e4c-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="40e4c-119">Remarks</span></span>

<span data-ttu-id="40e4c-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="40e4c-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="40e4c-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40e4c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40e4c-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="40e4c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40e4c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="40e4c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40e4c-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="40e4c-124">Schema name</span></span>  <br/> |<span data-ttu-id="40e4c-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="40e4c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="40e4c-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="40e4c-126">Validation file</span></span>  <br/> |<span data-ttu-id="40e4c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40e4c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40e4c-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="40e4c-128">Can be empty</span></span>  <br/> ||
   

