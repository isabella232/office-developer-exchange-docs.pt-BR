---
title: Userparameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: O elemento Userparameters contém uma lista de extensões de cliente habilitadas e desabilitadas.
ms.openlocfilehash: 76bf858adfb6d2ef76a25c234117131752c60d7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526750"
---
# <a name="userparameters"></a><span data-ttu-id="ef7b7-103">Userparameters</span><span class="sxs-lookup"><span data-stu-id="ef7b7-103">UserParameters</span></span>

<span data-ttu-id="ef7b7-104">O elemento **userparameters** contém uma lista de extensões de cliente habilitadas e desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-104">The **UserParameters** element contains a list of enabled and disabled client extensions.</span></span> 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 <span data-ttu-id="ef7b7-105">**GetClientExtensionUserParametersType**</span><span class="sxs-lookup"><span data-stu-id="ef7b7-105">**GetClientExtensionUserParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef7b7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ef7b7-106">Attributes and elements</span></span>

<span data-ttu-id="ef7b7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef7b7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef7b7-108">Attributes</span></span>

|<span data-ttu-id="ef7b7-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ef7b7-109">**Attribute**</span></span>|<span data-ttu-id="ef7b7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef7b7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef7b7-111">UserId</span><span class="sxs-lookup"><span data-stu-id="ef7b7-111">UserId</span></span>  <br/> |<span data-ttu-id="ef7b7-112">O valor de texto do atributo **userid** é o identificador do usuário.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-112">The text value of the **UserId** attribute is the identifier of the user.</span></span>  <br/> |
|<span data-ttu-id="ef7b7-113">EnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ef7b7-113">EnabledOnly</span></span>  <br/> |<span data-ttu-id="ef7b7-114">O valor de texto de **EnabledOnly** indica se a resposta contém apenas as extensões habilitadas.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-114">The text value of the **EnabledOnly** indicates whether the response only contains the enabled extensions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef7b7-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef7b7-115">Child elements</span></span>

<span data-ttu-id="ef7b7-116">[UserEnabledExtensions](userenabledextensions.md)  |  [UserDisabledExtensions](userdisabledextensions.md)</span><span class="sxs-lookup"><span data-stu-id="ef7b7-116">[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef7b7-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef7b7-117">Parent elements</span></span>

[<span data-ttu-id="ef7b7-118">GetClientExtension</span><span class="sxs-lookup"><span data-stu-id="ef7b7-118">GetClientExtension</span></span>](getclientextension.md)
  
## <a name="remarks"></a><span data-ttu-id="ef7b7-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef7b7-119">Remarks</span></span>

<span data-ttu-id="ef7b7-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ef7b7-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef7b7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef7b7-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ef7b7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef7b7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef7b7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef7b7-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef7b7-124">Schema name</span></span>  <br/> |<span data-ttu-id="ef7b7-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ef7b7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef7b7-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef7b7-126">Validation file</span></span>  <br/> |<span data-ttu-id="ef7b7-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ef7b7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef7b7-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ef7b7-128">Can be empty</span></span>  <br/> ||
   

