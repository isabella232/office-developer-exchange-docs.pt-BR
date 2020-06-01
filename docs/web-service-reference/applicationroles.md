---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: O elemento ApplicationRoles especifica as funções de aplicativo que o aplicativo de parceiro de chamada usa para a chamada atual.
ms.openlocfilehash: 8dfe5c745896d02217cbf91375d355954a4e22eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464697"
---
# <a name="applicationroles"></a><span data-ttu-id="faecf-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="faecf-103">ApplicationRoles</span></span>

<span data-ttu-id="faecf-104">O elemento **ApplicationRoles** especifica as funções de aplicativo que o aplicativo de parceiro de chamada usa para a chamada atual.</span><span class="sxs-lookup"><span data-stu-id="faecf-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="faecf-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="faecf-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faecf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="faecf-106">Attributes and elements</span></span>

<span data-ttu-id="faecf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="faecf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faecf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="faecf-108">Attributes</span></span>

<span data-ttu-id="faecf-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faecf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="faecf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="faecf-110">Child elements</span></span>

|<span data-ttu-id="faecf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="faecf-111">**Element**</span></span>|<span data-ttu-id="faecf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="faecf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faecf-113">Função</span><span class="sxs-lookup"><span data-stu-id="faecf-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="faecf-114">Especifica uma cadeia de caracteres que representa uma função de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="faecf-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="faecf-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="faecf-115">Parent elements</span></span>

|<span data-ttu-id="faecf-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="faecf-116">**Element**</span></span>|<span data-ttu-id="faecf-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="faecf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faecf-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="faecf-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="faecf-119">Especifica a função de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="faecf-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="faecf-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="faecf-120">Remarks</span></span>

<span data-ttu-id="faecf-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="faecf-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="faecf-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="faecf-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faecf-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="faecf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faecf-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="faecf-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="faecf-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="faecf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="faecf-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="faecf-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="faecf-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="faecf-127">Validation File</span></span>  <br/> |<span data-ttu-id="faecf-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="faecf-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="faecf-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="faecf-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="faecf-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="faecf-130">See also</span></span>

- [<span data-ttu-id="faecf-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="faecf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

