---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: O elemento MovedItemId Especifica o identificador do item que foi movido pela operação de MarkAsJunk.
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824484"
---
# <a name="moveditemid"></a><span data-ttu-id="53dea-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="53dea-103">MovedItemId</span></span>

<span data-ttu-id="53dea-104">O elemento **MovedItemId** Especifica o identificador do item que foi movido pela operação de **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="53dea-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="53dea-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="53dea-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53dea-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="53dea-106">Attributes and elements</span></span>

<span data-ttu-id="53dea-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53dea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53dea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53dea-108">Attributes</span></span>

|<span data-ttu-id="53dea-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="53dea-109">**Attribute**</span></span>|<span data-ttu-id="53dea-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53dea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53dea-111">Id</span><span class="sxs-lookup"><span data-stu-id="53dea-111">Id</span></span>  <br/> |<span data-ttu-id="53dea-112">O valor do atributo **Id** é o identificador de item do item que é movido pela operação de **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="53dea-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="53dea-113">O identificador do item permanecerá inalterado o mesmo após a migração.</span><span class="sxs-lookup"><span data-stu-id="53dea-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="53dea-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="53dea-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="53dea-115">O valor do atributo **ChangeKey** é a chave de alteração do item movido.</span><span class="sxs-lookup"><span data-stu-id="53dea-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="53dea-116">A chave de alteração é alterado depois que o item é movido pela operação de **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="53dea-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="53dea-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53dea-117">Child elements</span></span>

<span data-ttu-id="53dea-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53dea-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53dea-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53dea-119">Parent elements</span></span>

[<span data-ttu-id="53dea-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="53dea-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="53dea-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="53dea-121">Remarks</span></span>

<span data-ttu-id="53dea-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="53dea-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="53dea-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53dea-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53dea-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="53dea-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53dea-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="53dea-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="53dea-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53dea-126">Schema name</span></span>  <br/> |<span data-ttu-id="53dea-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="53dea-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="53dea-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53dea-128">Validation file</span></span>  <br/> |<span data-ttu-id="53dea-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="53dea-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53dea-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="53dea-130">Can be empty</span></span>  <br/> ||
   

