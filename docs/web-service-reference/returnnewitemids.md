---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: O elemento ReturnNewItemIds indica se os identificadores de item de novos itens são retornados na resposta.
ms.openlocfilehash: 003676c4c034454aa551e42bf3af976183117b8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465111"
---
# <a name="returnnewitemids"></a><span data-ttu-id="c8f89-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="c8f89-103">ReturnNewItemIds</span></span>

<span data-ttu-id="c8f89-104">O elemento **ReturnNewItemIds** indica se os identificadores de item de novos itens são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f89-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="c8f89-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="c8f89-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8f89-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c8f89-106">Attributes and elements</span></span>

<span data-ttu-id="c8f89-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8f89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8f89-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8f89-108">Attributes</span></span>

<span data-ttu-id="c8f89-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8f89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8f89-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8f89-110">Child elements</span></span>

<span data-ttu-id="c8f89-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8f89-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8f89-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8f89-112">Parent elements</span></span>

|<span data-ttu-id="c8f89-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8f89-113">**Element**</span></span>|<span data-ttu-id="c8f89-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8f89-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8f89-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="c8f89-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="c8f89-116">Define uma solicitação para copiar um item em uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8f89-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c8f89-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="c8f89-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="c8f89-118">Define uma solicitação para mover um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8f89-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8f89-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c8f89-119">Text value</span></span>

<span data-ttu-id="c8f89-120">Um valor de texto **true** para o elemento **ReturnNewItemIds** indica que os novos identificadores de item são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f89-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="c8f89-121">Um valor **false** indica que os novos identificadores de item não são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="c8f89-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c8f89-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c8f89-122">Remarks</span></span>

<span data-ttu-id="c8f89-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c8f89-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8f89-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c8f89-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8f89-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8f89-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c8f89-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c8f89-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c8f89-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c8f89-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="c8f89-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c8f89-128">Validation File</span></span>  <br/> |<span data-ttu-id="c8f89-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c8f89-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8f89-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c8f89-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8f89-131">Falso</span><span class="sxs-lookup"><span data-stu-id="c8f89-131">False</span></span>  <br/> |
   

