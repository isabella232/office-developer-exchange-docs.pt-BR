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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466028"
---
# <a name="userconfigurationname"></a><span data-ttu-id="1c312-104">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="1c312-104">UserConfigurationName</span></span>

<span data-ttu-id="1c312-105">O elemento **Userconfigurationname** representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="1c312-106">O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
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

<span data-ttu-id="1c312-107">**Userconfigurationtype**</span><span class="sxs-lookup"><span data-stu-id="1c312-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1c312-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1c312-108">Attributes and elements</span></span>

<span data-ttu-id="1c312-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1c312-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c312-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1c312-110">Attributes</span></span>

|<span data-ttu-id="1c312-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="1c312-111">**Attribute**</span></span>|<span data-ttu-id="1c312-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c312-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c312-113">**Nome**</span><span class="sxs-lookup"><span data-stu-id="1c312-113">**Name**</span></span> <br/> |<span data-ttu-id="1c312-114">Contém um valor String que representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="1c312-115">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="1c312-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1c312-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1c312-116">Child elements</span></span>

|<span data-ttu-id="1c312-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c312-117">**Element**</span></span>|<span data-ttu-id="1c312-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c312-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c312-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="1c312-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="1c312-120">Representa o identificador de pasta da pasta que contém o objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="1c312-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="1c312-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="1c312-122">Representa um nome de pasta distinta da pasta que contém o objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c312-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1c312-123">Parent elements</span></span>

|<span data-ttu-id="1c312-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c312-124">**Element**</span></span>|<span data-ttu-id="1c312-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c312-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c312-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c312-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="1c312-127">Representa uma solicitação para excluir um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="1c312-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c312-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="1c312-129">Representa uma solicitação para obter um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="1c312-130">Userconfiguration</span><span class="sxs-lookup"><span data-stu-id="1c312-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="1c312-131">Define um único objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="1c312-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c312-132">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1c312-132">Text value</span></span>

<span data-ttu-id="1c312-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1c312-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1c312-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c312-134">Remarks</span></span>

<span data-ttu-id="1c312-135">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c312-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c312-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1c312-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c312-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c312-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c312-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1c312-138">Schema Name</span></span>  <br/> |<span data-ttu-id="1c312-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1c312-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c312-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1c312-140">Validation File</span></span>  <br/> |<span data-ttu-id="1c312-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1c312-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c312-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1c312-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c312-143">False</span><span class="sxs-lookup"><span data-stu-id="1c312-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c312-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="1c312-144">See also</span></span>

- [<span data-ttu-id="1c312-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1c312-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

