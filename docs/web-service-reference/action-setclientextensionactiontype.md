---
title: Ação (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: O elemento Action contém a ação que o Exchange server deve ser adotada em um aplicativo.
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751041"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="6d03d-103">Ação (SetClientExtensionActionType)</span><span class="sxs-lookup"><span data-stu-id="6d03d-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="6d03d-104">O elemento **Action** contém a ação que o Exchange server deve ser adotada em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d03d-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="6d03d-105">**SetClientExtensionActionType**</span><span class="sxs-lookup"><span data-stu-id="6d03d-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d03d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6d03d-106">Attributes and elements</span></span>

<span data-ttu-id="6d03d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d03d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d03d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d03d-108">Attributes</span></span>

|<span data-ttu-id="6d03d-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="6d03d-109">**Attribute**</span></span>|<span data-ttu-id="6d03d-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d03d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d03d-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="6d03d-111">ActionId</span></span>  <br/> |<span data-ttu-id="6d03d-112">Especifica o identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="6d03d-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="6d03d-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6d03d-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6d03d-114">ExtensionId</span><span class="sxs-lookup"><span data-stu-id="6d03d-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="6d03d-115">Especifica o identificador da extensão.</span><span class="sxs-lookup"><span data-stu-id="6d03d-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="6d03d-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="6d03d-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="6d03d-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="6d03d-117">ActionId</span></span>

|<span data-ttu-id="6d03d-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6d03d-118">**Value**</span></span>|<span data-ttu-id="6d03d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d03d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d03d-120">Configurar</span><span class="sxs-lookup"><span data-stu-id="6d03d-120">Configure</span></span>  <br/> |<span data-ttu-id="6d03d-121">Indica uma ação de configuração.</span><span class="sxs-lookup"><span data-stu-id="6d03d-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="6d03d-122">Instalar</span><span class="sxs-lookup"><span data-stu-id="6d03d-122">Install</span></span>  <br/> |<span data-ttu-id="6d03d-123">Indica uma ação de instalação.</span><span class="sxs-lookup"><span data-stu-id="6d03d-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="6d03d-124">Desinstalar</span><span class="sxs-lookup"><span data-stu-id="6d03d-124">Uninstall</span></span>  <br/> |<span data-ttu-id="6d03d-125">Indica uma ação de desinstalação.</span><span class="sxs-lookup"><span data-stu-id="6d03d-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6d03d-126">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d03d-126">Child elements</span></span>

|<span data-ttu-id="6d03d-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d03d-127">**Element**</span></span>|<span data-ttu-id="6d03d-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d03d-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d03d-129">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="6d03d-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="6d03d-130">Contém informações de usuário e de configuração sobre um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d03d-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d03d-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d03d-131">Parent elements</span></span>

|<span data-ttu-id="6d03d-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d03d-132">**Element**</span></span>|<span data-ttu-id="6d03d-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d03d-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d03d-134">Ações (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="6d03d-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="6d03d-135">Especifica uma matriz de elementos de **ação** .</span><span class="sxs-lookup"><span data-stu-id="6d03d-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d03d-136">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="6d03d-136">Remarks</span></span>

<span data-ttu-id="6d03d-137">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6d03d-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6d03d-138">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d03d-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d03d-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6d03d-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d03d-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d03d-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d03d-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6d03d-141">Schema Name</span></span>  <br/> |<span data-ttu-id="6d03d-142">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="6d03d-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="6d03d-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6d03d-143">Validation File</span></span>  <br/> |<span data-ttu-id="6d03d-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d03d-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d03d-145">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6d03d-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6d03d-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="6d03d-146">See also</span></span>

- [<span data-ttu-id="6d03d-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6d03d-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

