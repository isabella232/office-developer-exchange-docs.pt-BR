---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: O elemento SharingFolderId representa o identificador da pasta local em uma relação de compartilhamento.
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825485"
---
# <a name="sharingfolderid"></a><span data-ttu-id="66645-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="66645-103">SharingFolderId</span></span>

<span data-ttu-id="66645-104">O elemento **SharingFolderId** representa o identificador da pasta local em uma relação de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="66645-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="66645-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="66645-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66645-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="66645-106">Attributes and elements</span></span>

<span data-ttu-id="66645-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="66645-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66645-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="66645-108">Attributes</span></span>

|<span data-ttu-id="66645-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="66645-109">**Attribute**</span></span>|<span data-ttu-id="66645-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66645-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66645-111">Id</span><span class="sxs-lookup"><span data-stu-id="66645-111">Id</span></span>  <br/> |<span data-ttu-id="66645-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="66645-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="66645-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="66645-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="66645-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="66645-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="66645-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo Id.</span><span class="sxs-lookup"><span data-stu-id="66645-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="66645-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="66645-116">This attribute is optional.</span></span> <span data-ttu-id="66645-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="66645-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66645-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="66645-118">Child elements</span></span>

<span data-ttu-id="66645-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="66645-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66645-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="66645-120">Parent elements</span></span>

|<span data-ttu-id="66645-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66645-121">**Element**</span></span>|<span data-ttu-id="66645-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66645-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66645-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="66645-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="66645-124">Define uma solicitação para atualizar a pasta local especificada.</span><span class="sxs-lookup"><span data-stu-id="66645-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="66645-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="66645-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="66645-126">Define uma resposta a uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="66645-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="66645-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66645-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="66645-128">Contém o status e o resultado de uma única solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="66645-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66645-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="66645-129">Remarks</span></span>

<span data-ttu-id="66645-130">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="66645-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66645-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="66645-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66645-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="66645-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66645-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="66645-133">Schema Name</span></span>  <br/> |<span data-ttu-id="66645-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="66645-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66645-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="66645-135">Validation File</span></span>  <br/> |<span data-ttu-id="66645-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66645-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66645-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="66645-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="66645-138">False</span><span class="sxs-lookup"><span data-stu-id="66645-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66645-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="66645-139">See also</span></span>



- [<span data-ttu-id="66645-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66645-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

