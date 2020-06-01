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
description: O elemento RefreshSharingFolder define uma solicitação para atualizar a pasta local especificada. É o elemento base para a operação RefreshSharingFolder.
ms.openlocfilehash: 4454607fa2c3114cc7279fd7c30f8aee74707baa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467925"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="96404-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="96404-104">RefreshSharingFolder</span></span>

<span data-ttu-id="96404-105">O elemento **RefreshSharingFolder** define uma solicitação para atualizar a pasta local especificada.</span><span class="sxs-lookup"><span data-stu-id="96404-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="96404-106">É o elemento base para a [operação RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="96404-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="96404-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="96404-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96404-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96404-108">Attributes and elements</span></span>

<span data-ttu-id="96404-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96404-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96404-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="96404-110">Attributes</span></span>

<span data-ttu-id="96404-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96404-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96404-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96404-112">Child elements</span></span>

|<span data-ttu-id="96404-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96404-113">**Element**</span></span>|<span data-ttu-id="96404-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96404-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96404-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="96404-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="96404-116">Representa o identificador da pasta local em uma relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="96404-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96404-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96404-117">Parent elements</span></span>

<span data-ttu-id="96404-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96404-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96404-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="96404-119">Remarks</span></span>

<span data-ttu-id="96404-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="96404-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96404-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96404-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96404-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="96404-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96404-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96404-123">Schema Name</span></span>  <br/> |<span data-ttu-id="96404-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="96404-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96404-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96404-125">Validation File</span></span>  <br/> |<span data-ttu-id="96404-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96404-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96404-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96404-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="96404-128">False</span><span class="sxs-lookup"><span data-stu-id="96404-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96404-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="96404-129">See also</span></span>



- [<span data-ttu-id="96404-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96404-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

