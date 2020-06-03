---
title: MarkImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkImportance
api_type:
- schema
ms.assetid: 32b8b08f-65e9-4764-b40a-63245551f4a3
description: O elemento MarkImportance especifica a importância a ser carimbada nas mensagens.
ms.openlocfilehash: 051307c0943a22e0c46439410806d168603d8a69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530878"
---
# <a name="markimportance"></a><span data-ttu-id="ac920-103">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="ac920-103">MarkImportance</span></span>

<span data-ttu-id="ac920-104">O elemento **MarkImportance** especifica a importância a ser carimbada nas mensagens.</span><span class="sxs-lookup"><span data-stu-id="ac920-104">The **MarkImportance** element specifies the importance that is to be stamped on messages.</span></span> 
  
```XML
<MarkImportance/>
```

 <span data-ttu-id="ac920-105">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="ac920-105">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac920-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ac920-106">Attributes and elements</span></span>

<span data-ttu-id="ac920-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac920-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac920-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac920-108">Attributes</span></span>

<span data-ttu-id="ac920-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac920-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac920-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac920-110">Child elements</span></span>

<span data-ttu-id="ac920-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac920-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac920-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac920-112">Parent elements</span></span>

|<span data-ttu-id="ac920-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac920-113">**Element**</span></span>|<span data-ttu-id="ac920-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac920-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac920-115">Actions</span><span class="sxs-lookup"><span data-stu-id="ac920-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ac920-116">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="ac920-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac920-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ac920-117">Text value</span></span>

<span data-ttu-id="ac920-118">O valor de texto para esse elemento é restrito a um dos seguintes valores de cadeia de caracteres:</span><span class="sxs-lookup"><span data-stu-id="ac920-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="ac920-119">Baixo</span><span class="sxs-lookup"><span data-stu-id="ac920-119">Low</span></span>
    
- <span data-ttu-id="ac920-120">Normal</span><span class="sxs-lookup"><span data-stu-id="ac920-120">Normal</span></span>
    
- <span data-ttu-id="ac920-121">Alta</span><span class="sxs-lookup"><span data-stu-id="ac920-121">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ac920-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac920-122">Remarks</span></span>

<span data-ttu-id="ac920-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac920-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac920-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ac920-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac920-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac920-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac920-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ac920-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ac920-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ac920-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac920-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ac920-128">Validation File</span></span>  <br/> |<span data-ttu-id="ac920-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ac920-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac920-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ac920-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac920-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ac920-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac920-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="ac920-132">See also</span></span>



- [<span data-ttu-id="ac920-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ac920-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

