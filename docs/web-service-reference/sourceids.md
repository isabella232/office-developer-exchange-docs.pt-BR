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
description: O elemento SourceIds contém os identificadores de origem a serem convertidos.
ms.openlocfilehash: 1c4990f2185788c5cfaab5483cb6a54a0d850596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466105"
---
# <a name="sourceids"></a><span data-ttu-id="26aa0-103">SourceIds</span><span class="sxs-lookup"><span data-stu-id="26aa0-103">SourceIds</span></span>

<span data-ttu-id="26aa0-104">O elemento **SourceIds** contém os identificadores de origem a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="26aa0-104">The **SourceIds** element contains the source identifiers to convert.</span></span> 
  
[<span data-ttu-id="26aa0-105">ConvertId</span><span class="sxs-lookup"><span data-stu-id="26aa0-105">ConvertId</span></span>](convertid.md)
  
[<span data-ttu-id="26aa0-106">SourceIds</span><span class="sxs-lookup"><span data-stu-id="26aa0-106">SourceIds</span></span>](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 <span data-ttu-id="26aa0-107">**NonEmptyArrayOfAlternateIdsType**</span><span class="sxs-lookup"><span data-stu-id="26aa0-107">**NonEmptyArrayOfAlternateIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26aa0-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="26aa0-108">Attributes and elements</span></span>

<span data-ttu-id="26aa0-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26aa0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26aa0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="26aa0-110">Attributes</span></span>

<span data-ttu-id="26aa0-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26aa0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26aa0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26aa0-112">Child elements</span></span>

|<span data-ttu-id="26aa0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26aa0-113">**Element**</span></span>|<span data-ttu-id="26aa0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26aa0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26aa0-115">AlternateId</span><span class="sxs-lookup"><span data-stu-id="26aa0-115">AlternateId</span></span>](alternateid.md) <br/> |<span data-ttu-id="26aa0-116">Descreve um item ou identificador de pasta a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="26aa0-116">Describes an item or folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="26aa0-117">AlternatePublicFolderId</span><span class="sxs-lookup"><span data-stu-id="26aa0-117">AlternatePublicFolderId</span></span>](alternatepublicfolderid.md) <br/> |<span data-ttu-id="26aa0-118">Descreve um identificador de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="26aa0-118">Describes a public folder identifier to convert.</span></span>  <br/> |
|[<span data-ttu-id="26aa0-119">AlternatePublicFolderItemId</span><span class="sxs-lookup"><span data-stu-id="26aa0-119">AlternatePublicFolderItemId</span></span>](alternatepublicfolderitemid.md) <br/> |<span data-ttu-id="26aa0-120">Descreve um identificador de item de pasta pública a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="26aa0-120">Describes a public folder item identifier to convert.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26aa0-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26aa0-121">Parent elements</span></span>

|<span data-ttu-id="26aa0-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26aa0-122">**Element**</span></span>|<span data-ttu-id="26aa0-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26aa0-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26aa0-124">ConvertId</span><span class="sxs-lookup"><span data-stu-id="26aa0-124">ConvertId</span></span>](convertid.md) <br/> |<span data-ttu-id="26aa0-125">Define uma solicitação para converter os identificadores de item e de pasta entre os formatos com suporte do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26aa0-125">Defines a request to convert item and folder identifiers between Exchange supported formats.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26aa0-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="26aa0-126">Remarks</span></span>

<span data-ttu-id="26aa0-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="26aa0-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26aa0-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="26aa0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26aa0-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="26aa0-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26aa0-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26aa0-130">Schema Name</span></span>  <br/> |<span data-ttu-id="26aa0-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="26aa0-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26aa0-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26aa0-132">Validation File</span></span>  <br/> |<span data-ttu-id="26aa0-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="26aa0-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26aa0-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="26aa0-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="26aa0-135">False</span><span class="sxs-lookup"><span data-stu-id="26aa0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26aa0-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="26aa0-136">See also</span></span>



[<span data-ttu-id="26aa0-137">Operação convertid</span><span class="sxs-lookup"><span data-stu-id="26aa0-137">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="26aa0-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26aa0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="26aa0-139">Convertendo identificadores</span><span class="sxs-lookup"><span data-stu-id="26aa0-139">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

