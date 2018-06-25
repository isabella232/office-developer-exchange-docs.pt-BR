---
title: MustDisplayComment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MustDisplayComment
api_type:
- schema
ms.assetid: 11d4d3c3-4652-4ed4-9b29-a0b5f85b82b7
description: O elemento MustDisplayComment indica se o comentário de pasta gerenciada deve ser exibido.
ms.openlocfilehash: 9a7e6a88b77ff9f1fd82507b8320898c195cd190
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824502"
---
# <a name="mustdisplaycomment"></a><span data-ttu-id="be532-103">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="be532-103">MustDisplayComment</span></span>

<span data-ttu-id="be532-104">O elemento **MustDisplayComment** indica se o comentário de pasta gerenciada deve ser exibido.</span><span class="sxs-lookup"><span data-stu-id="be532-104">The **MustDisplayComment** element indicates whether the managed folder comment must be displayed.</span></span> 
  
```xml
<MustDisplayComment/>
```

 <span data-ttu-id="be532-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="be532-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be532-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="be532-106">Attributes and elements</span></span>

<span data-ttu-id="be532-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be532-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be532-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be532-108">Attributes</span></span>

<span data-ttu-id="be532-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be532-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be532-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be532-110">Child elements</span></span>

<span data-ttu-id="be532-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be532-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be532-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be532-112">Parent elements</span></span>

|<span data-ttu-id="be532-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="be532-113">**Element**</span></span>|<span data-ttu-id="be532-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be532-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be532-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="be532-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="be532-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="be532-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be532-117">Text value</span><span class="sxs-lookup"><span data-stu-id="be532-117">Text value</span></span>

<span data-ttu-id="be532-118">O valor de texto representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="be532-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="be532-119">Um valor **true** indica que o comentário deve ser exibido; um valor **false** indica que o comentário não tem a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="be532-119">A value of **true** indicates that the comment must be displayed; a value of **false** indicates that the comment does not have to be displayed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="be532-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="be532-120">Remarks</span></span>

<span data-ttu-id="be532-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="be532-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be532-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="be532-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be532-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="be532-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be532-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be532-124">Schema name</span></span>  <br/> |<span data-ttu-id="be532-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="be532-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="be532-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be532-126">Validation file</span></span>  <br/> |<span data-ttu-id="be532-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="be532-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be532-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="be532-128">Can be empty</span></span>  <br/> |<span data-ttu-id="be532-129">False</span><span class="sxs-lookup"><span data-stu-id="be532-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be532-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="be532-130">See also</span></span>



[<span data-ttu-id="be532-131">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="be532-131">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="be532-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be532-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

