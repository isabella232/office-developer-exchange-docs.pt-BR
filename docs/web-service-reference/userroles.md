---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: O elemento UserRoles especifica as funções de usuário que o usuário de chamada ou o usuário que o aplicativo de parceiro de chamada está agindo como, deseja aplicar à chamada atual.
ms.openlocfilehash: 5155b82781321b16d1b58fdcaffe7b8cf2372717
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467127"
---
# <a name="userroles"></a><span data-ttu-id="34f61-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="34f61-103">UserRoles</span></span>

<span data-ttu-id="34f61-104">O elemento **UserRoles** especifica as funções de usuário que o usuário de chamada ou o usuário que o aplicativo de parceiro de chamada está agindo como, deseja aplicar à chamada atual.</span><span class="sxs-lookup"><span data-stu-id="34f61-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="34f61-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="34f61-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34f61-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="34f61-106">Attributes and elements</span></span>

<span data-ttu-id="34f61-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="34f61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34f61-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="34f61-108">Attributes</span></span>

<span data-ttu-id="34f61-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34f61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34f61-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="34f61-110">Child elements</span></span>

[<span data-ttu-id="34f61-111">Função</span><span class="sxs-lookup"><span data-stu-id="34f61-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="34f61-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="34f61-112">Parent elements</span></span>

[<span data-ttu-id="34f61-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="34f61-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="34f61-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="34f61-114">Remarks</span></span>

<span data-ttu-id="34f61-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34f61-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34f61-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="34f61-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34f61-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="34f61-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34f61-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="34f61-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34f61-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="34f61-119">Schema name</span></span>  <br/> |<span data-ttu-id="34f61-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="34f61-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="34f61-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="34f61-121">Validation file</span></span>  <br/> |<span data-ttu-id="34f61-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="34f61-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34f61-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="34f61-123">Can be empty</span></span>  <br/> ||
   

