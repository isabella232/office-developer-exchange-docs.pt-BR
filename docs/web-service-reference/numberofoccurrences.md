---
title: NumberOfOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfOccurrences
api_type:
- schema
ms.assetid: 9ec86ceb-b271-4718-97ca-b6a532ea7223
description: O elemento NumberOfOccurrences contém o número de ocorrências de um item recorrente.
ms.openlocfilehash: f9b72611e87c5f2b98deb14c25988e574a324491
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462539"
---
# <a name="numberofoccurrences"></a><span data-ttu-id="96233-103">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="96233-103">NumberOfOccurrences</span></span>

<span data-ttu-id="96233-104">O elemento **NumberOfOccurrences** contém o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="96233-104">The **NumberOfOccurrences** element contains the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberOfOccurrences/>
```

 <span data-ttu-id="96233-105">**int**</span><span class="sxs-lookup"><span data-stu-id="96233-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96233-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96233-106">Attributes and elements</span></span>

<span data-ttu-id="96233-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96233-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96233-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="96233-108">Attributes</span></span>

<span data-ttu-id="96233-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96233-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96233-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96233-110">Child elements</span></span>

<span data-ttu-id="96233-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96233-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96233-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96233-112">Parent elements</span></span>

|<span data-ttu-id="96233-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96233-113">**Element**</span></span>|<span data-ttu-id="96233-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96233-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96233-115">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="96233-115">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="96233-116">Descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="96233-116">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96233-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="96233-117">Text value</span></span>

<span data-ttu-id="96233-118">O valor de texto é um inteiro que representa o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="96233-118">The text value is an integer that represents the number of occurrences of a recurring item.</span></span> <span data-ttu-id="96233-119">O valor deve ser um inteiro no intervalo de 1 a 999.</span><span class="sxs-lookup"><span data-stu-id="96233-119">The value must be an integer in the range of 1 to 999.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96233-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="96233-120">Remarks</span></span>

<span data-ttu-id="96233-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="96233-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96233-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96233-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96233-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="96233-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96233-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96233-124">Schema name</span></span>  <br/> |<span data-ttu-id="96233-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="96233-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="96233-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96233-126">Validation file</span></span>  <br/> |<span data-ttu-id="96233-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="96233-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96233-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="96233-128">Can be empty</span></span>  <br/> |<span data-ttu-id="96233-129">False</span><span class="sxs-lookup"><span data-stu-id="96233-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96233-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="96233-130">See also</span></span>



- [<span data-ttu-id="96233-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96233-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

