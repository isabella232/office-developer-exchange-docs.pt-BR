---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: O elemento de AddNewImContactToGroup define uma solicitação para adicionar um novo contato de mensagens instantâneo a um grupo de mensagens instantâneo.
ms.openlocfilehash: 2736bac6880a11101e9bffee12033c838705700e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751058"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="73aef-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="73aef-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="73aef-104">O elemento de **AddNewImContactToGroup** define uma solicitação para adicionar um novo contato de mensagens instantâneo a um grupo de mensagens instantâneo.</span><span class="sxs-lookup"><span data-stu-id="73aef-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="73aef-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="73aef-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73aef-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="73aef-106">Attributes and elements</span></span>

<span data-ttu-id="73aef-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="73aef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73aef-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="73aef-108">Attributes</span></span>

<span data-ttu-id="73aef-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73aef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73aef-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="73aef-110">Child elements</span></span>

<span data-ttu-id="73aef-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="73aef-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73aef-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="73aef-112">Parent elements</span></span>

<span data-ttu-id="73aef-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73aef-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73aef-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="73aef-114">Remarks</span></span>

<span data-ttu-id="73aef-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73aef-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="73aef-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="73aef-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73aef-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="73aef-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73aef-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="73aef-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73aef-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="73aef-119">Schema name</span></span>  <br/> |<span data-ttu-id="73aef-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="73aef-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73aef-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="73aef-121">Validation file</span></span>  <br/> |<span data-ttu-id="73aef-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73aef-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73aef-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="73aef-123">Can be empty</span></span>  <br/> |<span data-ttu-id="73aef-124">false</span><span class="sxs-lookup"><span data-stu-id="73aef-124">false</span></span>  <br/> |
   

