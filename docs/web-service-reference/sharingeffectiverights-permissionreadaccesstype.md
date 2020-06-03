---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: O elemento SharingEffectiveRights indica as permissões que o usuário tem para os dados de contato que estão sendo compartilhados.
ms.openlocfilehash: 64b1e6d831068e9699e9cd47693e74919e0416a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526659"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a><span data-ttu-id="c6e7c-103">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="c6e7c-103">SharingEffectiveRights (PermissionReadAccessType)</span></span>

<span data-ttu-id="c6e7c-104">O elemento **SharingEffectiveRights** indica as permissões que o usuário tem para os dados de contato que estão sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-104">The **SharingEffectiveRights** element indicates the permissions that the user has for the contact data that is being shared.</span></span> 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 <span data-ttu-id="c6e7c-105">**PermissionReadAccessType**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-105">**PermissionReadAccessType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6e7c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c6e7c-106">Attributes and elements</span></span>

<span data-ttu-id="c6e7c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6e7c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c6e7c-108">Attributes</span></span>

<span data-ttu-id="c6e7c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6e7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6e7c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c6e7c-110">Child elements</span></span>

<span data-ttu-id="c6e7c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6e7c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c6e7c-112">Parent elements</span></span>

|<span data-ttu-id="c6e7c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-113">**Element**</span></span>|<span data-ttu-id="c6e7c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6e7c-115">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c6e7c-115">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c6e7c-116">Representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-116">Represents a Contacts folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6e7c-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c6e7c-117">Text value</span></span>

<span data-ttu-id="c6e7c-118">A tabela a seguir lista os valores possíveis para o elemento **SharingEffectiveRights** .</span><span class="sxs-lookup"><span data-stu-id="c6e7c-118">The following table lists the possible values for the **SharingEffectiveRights** element.</span></span> 
  
<span data-ttu-id="c6e7c-119">**Valores de texto do elemento SharingEffectiveRights**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-119">**SharingEffectiveRights element text values**</span></span>

|<span data-ttu-id="c6e7c-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-120">**Value**</span></span>|<span data-ttu-id="c6e7c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6e7c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6e7c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6e7c-122">None</span></span>  <br/> |<span data-ttu-id="c6e7c-123">Indica que o usuário não tem permissão para ler itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-123">Indicates that the user does not have permission to read items in the folder.</span></span>  <br/> |
|<span data-ttu-id="c6e7c-124">FullDetails</span><span class="sxs-lookup"><span data-stu-id="c6e7c-124">FullDetails</span></span>  <br/> |<span data-ttu-id="c6e7c-125">Indica que o usuário tem permissão para ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-125">Indicates that the user has permission to read all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6e7c-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6e7c-126">Remarks</span></span>

<span data-ttu-id="c6e7c-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6e7c-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6e7c-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c6e7c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6e7c-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6e7c-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6e7c-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c6e7c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c6e7c-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c6e7c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6e7c-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c6e7c-132">Validation File</span></span>  <br/> |<span data-ttu-id="c6e7c-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c6e7c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6e7c-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c6e7c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6e7c-135">False</span><span class="sxs-lookup"><span data-stu-id="c6e7c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6e7c-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="c6e7c-136">See also</span></span>



- [<span data-ttu-id="c6e7c-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c6e7c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

