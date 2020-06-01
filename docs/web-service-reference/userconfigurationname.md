---
title: Userconfigurationname
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: O elemento userconfigurationname representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466028"
---
# <a name="userconfigurationname"></a><span data-ttu-id="097ea-104">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="097ea-104">UserConfigurationName</span></span>

<span data-ttu-id="097ea-105">O elemento **Userconfigurationname** representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="097ea-106">O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

<span data-ttu-id="097ea-107">**Userconfigurationtype**</span><span class="sxs-lookup"><span data-stu-id="097ea-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="097ea-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="097ea-108">Attributes and elements</span></span>

<span data-ttu-id="097ea-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="097ea-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="097ea-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="097ea-110">Attributes</span></span>

|<span data-ttu-id="097ea-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="097ea-111">**Attribute**</span></span>|<span data-ttu-id="097ea-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097ea-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097ea-113">**Nome**</span><span class="sxs-lookup"><span data-stu-id="097ea-113">**Name**</span></span> <br/> |<span data-ttu-id="097ea-114">Contém um valor String que representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="097ea-115">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="097ea-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="097ea-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="097ea-116">Child elements</span></span>

|<span data-ttu-id="097ea-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097ea-117">**Element**</span></span>|<span data-ttu-id="097ea-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097ea-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097ea-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="097ea-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="097ea-120">Representa o identificador de pasta da pasta que contém o objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="097ea-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="097ea-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="097ea-122">Representa um nome de pasta distinta da pasta que contém o objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="097ea-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="097ea-123">Parent elements</span></span>

|<span data-ttu-id="097ea-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="097ea-124">**Element**</span></span>|<span data-ttu-id="097ea-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="097ea-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="097ea-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="097ea-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="097ea-127">Representa uma solicitação para excluir um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="097ea-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="097ea-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="097ea-129">Representa uma solicitação para obter um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="097ea-130">Userconfiguration</span><span class="sxs-lookup"><span data-stu-id="097ea-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="097ea-131">Define um único objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="097ea-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="097ea-132">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="097ea-132">Text value</span></span>

<span data-ttu-id="097ea-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="097ea-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="097ea-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="097ea-134">Remarks</span></span>

<span data-ttu-id="097ea-135">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="097ea-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="097ea-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="097ea-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="097ea-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="097ea-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="097ea-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="097ea-138">Schema Name</span></span>  <br/> |<span data-ttu-id="097ea-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="097ea-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="097ea-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="097ea-140">Validation File</span></span>  <br/> |<span data-ttu-id="097ea-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="097ea-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="097ea-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="097ea-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="097ea-143">False</span><span class="sxs-lookup"><span data-stu-id="097ea-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="097ea-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="097ea-144">See also</span></span>

- [<span data-ttu-id="097ea-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="097ea-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

