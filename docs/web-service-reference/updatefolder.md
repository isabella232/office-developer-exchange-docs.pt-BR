---
title: UpdateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 412d0683-2819-40c5-a0ae-f613499a7b66
description: O elemento UpdateFolder representa a operação que é usada para atualizar as propriedades de uma pasta especificada.
ms.openlocfilehash: 124ffd02a5ea2e7bf6f21cc7009dde08837906f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457043"
---
# <a name="updatefolder"></a><span data-ttu-id="0433d-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="0433d-103">UpdateFolder</span></span>

<span data-ttu-id="0433d-104">O elemento **UpdateFolder** representa a operação que é usada para atualizar as propriedades de uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="0433d-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="0433d-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="0433d-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0433d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0433d-106">Attributes and elements</span></span>

<span data-ttu-id="0433d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0433d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0433d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0433d-108">Attributes</span></span>

<span data-ttu-id="0433d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0433d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0433d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0433d-110">Child elements</span></span>

|<span data-ttu-id="0433d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0433d-111">**Element**</span></span>|<span data-ttu-id="0433d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0433d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0433d-113">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="0433d-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="0433d-114">Contém uma coleção de alterações para uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="0433d-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0433d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0433d-115">Parent elements</span></span>

<span data-ttu-id="0433d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0433d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0433d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="0433d-117">Remarks</span></span>

<span data-ttu-id="0433d-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0433d-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0433d-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0433d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0433d-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="0433d-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0433d-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0433d-121">Schema Name</span></span>  <br/> |<span data-ttu-id="0433d-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0433d-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0433d-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0433d-123">Validation File</span></span>  <br/> |<span data-ttu-id="0433d-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0433d-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0433d-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0433d-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="0433d-126">False</span><span class="sxs-lookup"><span data-stu-id="0433d-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0433d-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="0433d-127">See also</span></span>



[<span data-ttu-id="0433d-128">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="0433d-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

