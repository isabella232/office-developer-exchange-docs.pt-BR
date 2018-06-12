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
ms.openlocfilehash: b70b28bd6b3c9452f5d7f249f453218d555754da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751375"
---
# <a name="candelete"></a><span data-ttu-id="16d11-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="16d11-103">CanDelete</span></span>

<span data-ttu-id="16d11-104">O elemento **CanDelete** indica se uma pasta gerenciada pode ser excluída por um cliente.</span><span class="sxs-lookup"><span data-stu-id="16d11-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="16d11-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="16d11-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16d11-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="16d11-106">Attributes and elements</span></span>

<span data-ttu-id="16d11-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="16d11-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16d11-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="16d11-108">Attributes</span></span>

<span data-ttu-id="16d11-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16d11-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16d11-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="16d11-110">Child elements</span></span>

<span data-ttu-id="16d11-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16d11-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16d11-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="16d11-112">Parent elements</span></span>

|<span data-ttu-id="16d11-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="16d11-113">**Element**</span></span>|<span data-ttu-id="16d11-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16d11-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16d11-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="16d11-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="16d11-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="16d11-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16d11-117">Text value</span><span class="sxs-lookup"><span data-stu-id="16d11-117">Text value</span></span>

<span data-ttu-id="16d11-118">Um valor de texto que representa um valor booleano é necessário se este elemento está presente.</span><span class="sxs-lookup"><span data-stu-id="16d11-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="16d11-119">Um valor **true** indica que a pasta pode ser excluída; um valor **false** significa que a pasta não pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="16d11-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="16d11-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="16d11-120">Remarks</span></span>

<span data-ttu-id="16d11-121">Para excluir uma pasta gerenciada, use a [operação DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="16d11-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="16d11-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="16d11-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16d11-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="16d11-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16d11-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="16d11-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16d11-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="16d11-125">Schema name</span></span>  <br/> |<span data-ttu-id="16d11-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="16d11-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="16d11-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="16d11-127">Validation file</span></span>  <br/> |<span data-ttu-id="16d11-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16d11-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16d11-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="16d11-129">Can be empty</span></span>  <br/> |<span data-ttu-id="16d11-130">False</span><span class="sxs-lookup"><span data-stu-id="16d11-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16d11-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="16d11-131">See also</span></span>



[<span data-ttu-id="16d11-132">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="16d11-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="16d11-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="16d11-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="16d11-134">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="16d11-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

