---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: O elemento SourceIds contém os identificadores de origem para converter.
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825522"
---
# <a name="sourceids"></a><span data-ttu-id="ff83e-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ff83e-103">SourceIds</span></span>

<span data-ttu-id="ff83e-104">O elemento **SourceIds** contém os identificadores de origem para converter.</span><span class="sxs-lookup"><span data-stu-id="ff83e-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="ff83e-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ff83e-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="ff83e-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="ff83e-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="ff83e-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="ff83e-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff83e-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ff83e-108">Attributes and elements</span></span>

<span data-ttu-id="ff83e-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff83e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff83e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff83e-110">Attributes</span></span>

<span data-ttu-id="ff83e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ff83e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff83e-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff83e-112">Child elements</span></span>

|<span data-ttu-id="ff83e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff83e-113">**Element**</span></span>|<span data-ttu-id="ff83e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff83e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff83e-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="ff83e-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="ff83e-116">Descreve um identificador de item ou pasta para converter.</span><span class="sxs-lookup"><span data-stu-id="ff83e-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="ff83e-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="ff83e-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="ff83e-118">Descreve um identificador de pasta pública para converter.</span><span class="sxs-lookup"><span data-stu-id="ff83e-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="ff83e-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="ff83e-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="ff83e-120">Descreve um identificador de item de pasta pública para converter.</span><span class="sxs-lookup"><span data-stu-id="ff83e-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff83e-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff83e-121">Parent elements</span></span>

|<span data-ttu-id="ff83e-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ff83e-122">**Element**</span></span>|<span data-ttu-id="ff83e-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ff83e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff83e-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="ff83e-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="ff83e-125">Define uma solicitação para converter os identificadores de item e pasta entre os formatos de suporte do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff83e-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff83e-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ff83e-126">Remarks</span></span>

<span data-ttu-id="ff83e-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ff83e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff83e-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ff83e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff83e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff83e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff83e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff83e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ff83e-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ff83e-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff83e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff83e-132">Validation File</span></span>  <br/> |<span data-ttu-id="ff83e-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff83e-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff83e-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ff83e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff83e-135">False</span><span class="sxs-lookup"><span data-stu-id="ff83e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff83e-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="ff83e-136">See also</span></span>



[<span data-ttu-id="ff83e-137">Operação ConvertId</span><span class="sxs-lookup"><span data-stu-id="ff83e-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="ff83e-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ff83e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ff83e-139">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="ff83e-139">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

