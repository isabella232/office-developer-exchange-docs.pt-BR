---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: O elemento de RefreshSharingFolder define uma solicitação para atualizar a pasta local especificada. É o elemento de base para a operação RefreshSharingFolder.
ms.openlocfilehash: b09e311d0ba38b0cdcc9fe0864ed3e2b0151b0fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825043"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="7153e-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="7153e-104">RefreshSharingFolder</span></span>

<span data-ttu-id="7153e-105">O elemento de **RefreshSharingFolder** define uma solicitação para atualizar a pasta local especificada.</span><span class="sxs-lookup"><span data-stu-id="7153e-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="7153e-106">É o elemento de base para a [operação RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7153e-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="7153e-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="7153e-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7153e-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7153e-108">Attributes and elements</span></span>

<span data-ttu-id="7153e-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7153e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7153e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7153e-110">Attributes</span></span>

<span data-ttu-id="7153e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7153e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7153e-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7153e-112">Child elements</span></span>

|<span data-ttu-id="7153e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7153e-113">**Element**</span></span>|<span data-ttu-id="7153e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7153e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7153e-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="7153e-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="7153e-116">Representa o identificador da pasta local em uma relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="7153e-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7153e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7153e-117">Parent elements</span></span>

<span data-ttu-id="7153e-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7153e-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7153e-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="7153e-119">Remarks</span></span>

<span data-ttu-id="7153e-120">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7153e-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7153e-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7153e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7153e-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="7153e-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7153e-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7153e-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7153e-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7153e-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7153e-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7153e-125">Validation File</span></span>  <br/> |<span data-ttu-id="7153e-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7153e-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7153e-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7153e-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7153e-128">False</span><span class="sxs-lookup"><span data-stu-id="7153e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7153e-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="7153e-129">See also</span></span>



- [<span data-ttu-id="7153e-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7153e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

