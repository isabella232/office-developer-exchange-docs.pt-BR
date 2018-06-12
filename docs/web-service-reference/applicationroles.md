---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: O elemento ApplicationRoles Especifica as funções do aplicativo usados pelo aplicativo de parceiro a chamada para a chamada atual.
ms.openlocfilehash: ff32b693dae573416263bcb7c0fbb552a933b8d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751102"
---
# <a name="applicationroles"></a><span data-ttu-id="690b6-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="690b6-103">ApplicationRoles</span></span>

<span data-ttu-id="690b6-104">O elemento **ApplicationRoles** Especifica as funções do aplicativo usados pelo aplicativo de parceiro a chamada para a chamada atual.</span><span class="sxs-lookup"><span data-stu-id="690b6-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="690b6-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="690b6-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="690b6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="690b6-106">Attributes and elements</span></span>

<span data-ttu-id="690b6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="690b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="690b6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="690b6-108">Attributes</span></span>

<span data-ttu-id="690b6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="690b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="690b6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="690b6-110">Child elements</span></span>

|<span data-ttu-id="690b6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="690b6-111">**Element**</span></span>|<span data-ttu-id="690b6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="690b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="690b6-113">Role</span><span class="sxs-lookup"><span data-stu-id="690b6-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="690b6-114">Especifica uma cadeia de caracteres que representa uma função de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="690b6-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="690b6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="690b6-115">Parent elements</span></span>

|<span data-ttu-id="690b6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="690b6-116">**Element**</span></span>|<span data-ttu-id="690b6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="690b6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="690b6-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="690b6-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="690b6-119">Especifica a função de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="690b6-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="690b6-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="690b6-120">Remarks</span></span>

<span data-ttu-id="690b6-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="690b6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="690b6-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="690b6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="690b6-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="690b6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="690b6-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="690b6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="690b6-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="690b6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="690b6-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="690b6-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="690b6-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="690b6-127">Validation File</span></span>  <br/> |<span data-ttu-id="690b6-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="690b6-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="690b6-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="690b6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="690b6-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="690b6-130">See also</span></span>

- [<span data-ttu-id="690b6-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="690b6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

