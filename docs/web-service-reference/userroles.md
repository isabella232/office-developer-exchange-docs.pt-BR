---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: O elemento UserRoles Especifica as funções de usuário que o usuário ou o usuário que o aplicativo de parceiro chamada está atuando como, quer aplicar para a chamada atual.
ms.openlocfilehash: 19dc1a7e00decb9141326b53b650d72101013c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837998"
---
# <a name="userroles"></a><span data-ttu-id="946fa-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="946fa-103">UserRoles</span></span>

<span data-ttu-id="946fa-104">O elemento **UserRoles** Especifica as funções de usuário que o usuário ou o usuário que o aplicativo de parceiro chamada está atuando como, quer aplicar para a chamada atual.</span><span class="sxs-lookup"><span data-stu-id="946fa-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="946fa-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="946fa-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="946fa-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="946fa-106">Attributes and elements</span></span>

<span data-ttu-id="946fa-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="946fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="946fa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="946fa-108">Attributes</span></span>

<span data-ttu-id="946fa-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="946fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="946fa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="946fa-110">Child elements</span></span>

[<span data-ttu-id="946fa-111">Role</span><span class="sxs-lookup"><span data-stu-id="946fa-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="946fa-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="946fa-112">Parent elements</span></span>

[<span data-ttu-id="946fa-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="946fa-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="946fa-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="946fa-114">Remarks</span></span>

<span data-ttu-id="946fa-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="946fa-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="946fa-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="946fa-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="946fa-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="946fa-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="946fa-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="946fa-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="946fa-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="946fa-119">Schema name</span></span>  <br/> |<span data-ttu-id="946fa-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="946fa-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="946fa-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="946fa-121">Validation file</span></span>  <br/> |<span data-ttu-id="946fa-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="946fa-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="946fa-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="946fa-123">Can be empty</span></span>  <br/> ||
   

