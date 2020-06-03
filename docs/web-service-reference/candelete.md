---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: O elemento CanDelete indica se uma pasta gerenciada pode ser excluída por um cliente.
ms.openlocfilehash: 5fe16c276bdb0c5b3b73ca63099559d3e869db3e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461587"
---
# <a name="candelete"></a><span data-ttu-id="fbafc-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="fbafc-103">CanDelete</span></span>

<span data-ttu-id="fbafc-104">O elemento **CanDelete** indica se uma pasta gerenciada pode ser excluída por um cliente.</span><span class="sxs-lookup"><span data-stu-id="fbafc-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="fbafc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fbafc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbafc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fbafc-106">Attributes and elements</span></span>

<span data-ttu-id="fbafc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fbafc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbafc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fbafc-108">Attributes</span></span>

<span data-ttu-id="fbafc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbafc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbafc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fbafc-110">Child elements</span></span>

<span data-ttu-id="fbafc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fbafc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbafc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fbafc-112">Parent elements</span></span>

|<span data-ttu-id="fbafc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fbafc-113">**Element**</span></span>|<span data-ttu-id="fbafc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fbafc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbafc-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="fbafc-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="fbafc-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="fbafc-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fbafc-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fbafc-117">Text value</span></span>

<span data-ttu-id="fbafc-118">Um valor de texto que representa um valor booliano é necessário se esse elemento estiver presente.</span><span class="sxs-lookup"><span data-stu-id="fbafc-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="fbafc-119">Um valor **true** indica que a pasta pode ser excluída; um valor **false** significa que a pasta não pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="fbafc-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fbafc-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="fbafc-120">Remarks</span></span>

<span data-ttu-id="fbafc-121">Para excluir uma pasta gerenciada, use a [operação DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fbafc-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="fbafc-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fbafc-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbafc-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fbafc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbafc-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="fbafc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbafc-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fbafc-125">Schema name</span></span>  <br/> |<span data-ttu-id="fbafc-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fbafc-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbafc-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fbafc-127">Validation file</span></span>  <br/> |<span data-ttu-id="fbafc-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fbafc-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbafc-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fbafc-129">Can be empty</span></span>  <br/> |<span data-ttu-id="fbafc-130">False</span><span class="sxs-lookup"><span data-stu-id="fbafc-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbafc-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="fbafc-131">See also</span></span>



[<span data-ttu-id="fbafc-132">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="fbafc-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="fbafc-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fbafc-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fbafc-134">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="fbafc-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

