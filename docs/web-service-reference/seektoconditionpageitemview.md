---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: O elemento SeekToConditionPageItemView identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para uma pesquisa do FindItem ou do FindConversation.
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466833"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="97665-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="97665-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="97665-104">O elemento **SeekToConditionPageItemView** identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para uma pesquisa do **FindItem** ou do **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="97665-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="97665-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="97665-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97665-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="97665-106">Attributes and elements</span></span>

<span data-ttu-id="97665-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97665-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97665-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97665-108">Attributes</span></span>

|<span data-ttu-id="97665-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="97665-109">**Attribute**</span></span>|<span data-ttu-id="97665-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97665-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97665-111">BasePoint</span><span class="sxs-lookup"><span data-stu-id="97665-111">BasePoint</span></span>  <br/> |<span data-ttu-id="97665-112">O valor de texto do atributo **BasePoint** é o ponto base de onde a pesquisa começará.</span><span class="sxs-lookup"><span data-stu-id="97665-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="97665-113">Um valor de texto **início** indica que a pesquisa começará no início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="97665-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="97665-114">Um valor de **fim** de texto indica que a pesquisa começará no final do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="97665-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="97665-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="97665-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="97665-116">O valor de texto do atributo **MaxEntriesReturned** é o número máximo de itens que podem ser retornados em um conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="97665-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97665-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97665-117">Child elements</span></span>

[<span data-ttu-id="97665-118">Condição (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="97665-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="97665-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97665-119">Parent elements</span></span>

<span data-ttu-id="97665-120">[FindConversation](findconversation.md)  |  [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="97665-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97665-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="97665-121">Remarks</span></span>

<span data-ttu-id="97665-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97665-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97665-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="97665-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97665-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="97665-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97665-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="97665-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97665-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97665-126">Schema name</span></span>  <br/> |<span data-ttu-id="97665-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="97665-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97665-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97665-128">Validation file</span></span>  <br/> |<span data-ttu-id="97665-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="97665-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97665-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="97665-130">Can be empty</span></span>  <br/> |<span data-ttu-id="97665-131">falso</span><span class="sxs-lookup"><span data-stu-id="97665-131">false</span></span>  <br/> |
   

