---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: O elemento SeekToConditionPageItemView identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma pesquisa FindItem ou FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825328"
---
# <a name="seektoconditionpageitemview"></a><span data-ttu-id="e258e-103">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="e258e-103">SeekToConditionPageItemView</span></span>

<span data-ttu-id="e258e-104">O elemento **SeekToConditionPageItemView** identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para um **FindItem** ou **FindConversation **pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e258e-104">The **SeekToConditionPageItemView** element identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span> 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 <span data-ttu-id="e258e-105">**SeekToConditionPageViewType**</span><span class="sxs-lookup"><span data-stu-id="e258e-105">**SeekToConditionPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e258e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e258e-106">Attributes and elements</span></span>

<span data-ttu-id="e258e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e258e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e258e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e258e-108">Attributes</span></span>

|<span data-ttu-id="e258e-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e258e-109">**Attribute**</span></span>|<span data-ttu-id="e258e-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e258e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e258e-111">Ponto de base</span><span class="sxs-lookup"><span data-stu-id="e258e-111">BasePoint</span></span>  <br/> |<span data-ttu-id="e258e-112">O valor de texto do atributo **ponto de base** é o ponto de base do qual a pesquisa será iniciada.</span><span class="sxs-lookup"><span data-stu-id="e258e-112">The text value of the **BasePoint** attribute is the base point from where the search will start.</span></span> <span data-ttu-id="e258e-113">Um valor de texto de **início** indica que a pesquisa começará no início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="e258e-113">A text value of **Beginning** indicates that the search will start at the beginning of the result set.</span></span> <span data-ttu-id="e258e-114">Um valor de texto do **final** indica que a pesquisa será iniciada no final do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="e258e-114">A text value of **End** indicates that the search will start at the end of the result set.</span></span>  <br/> |
|<span data-ttu-id="e258e-115">MaxEntriesReturned</span><span class="sxs-lookup"><span data-stu-id="e258e-115">MaxEntriesReturned</span></span>  <br/> |<span data-ttu-id="e258e-116">O valor de texto do atributo **MaxEntriesReturned** é o número máximo de itens que podem ser retornadas em um conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="e258e-116">The text value of the **MaxEntriesReturned** attribute is the maximum number of items that can be returned in a result set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e258e-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e258e-117">Child elements</span></span>

[<span data-ttu-id="e258e-118">Condição (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="e258e-118">Condition (RestrictionType)</span></span>](condition-restrictiontype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e258e-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e258e-119">Parent elements</span></span>

<span data-ttu-id="e258e-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span><span class="sxs-lookup"><span data-stu-id="e258e-120">[FindConversation](findconversation.md) | [FindItem](finditem.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e258e-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="e258e-121">Remarks</span></span>

<span data-ttu-id="e258e-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e258e-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e258e-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e258e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e258e-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e258e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e258e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e258e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e258e-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e258e-126">Schema name</span></span>  <br/> |<span data-ttu-id="e258e-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e258e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e258e-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e258e-128">Validation file</span></span>  <br/> |<span data-ttu-id="e258e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e258e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e258e-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e258e-130">Can be empty</span></span>  <br/> |<span data-ttu-id="e258e-131">false</span><span class="sxs-lookup"><span data-stu-id="e258e-131">false</span></span>  <br/> |
   

