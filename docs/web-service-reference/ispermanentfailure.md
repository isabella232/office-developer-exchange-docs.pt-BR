---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: O elemento IsPermanentFailure indica se uma tentativa anterior para indexar o item tiver sido bem sucedida.
ms.openlocfilehash: 39592c15394a57e1c6aa1183ed0ccedeb085e6ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824085"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="586bd-103">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="586bd-103">IsPermanentFailure</span></span>

<span data-ttu-id="586bd-104">O elemento **IsPermanentFailure** indica se uma tentativa anterior para indexar o item tiver sido bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="586bd-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="586bd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="586bd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="586bd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="586bd-106">Attributes and elements</span></span>

<span data-ttu-id="586bd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="586bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="586bd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="586bd-108">Attributes</span></span>

<span data-ttu-id="586bd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="586bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="586bd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="586bd-110">Child elements</span></span>

<span data-ttu-id="586bd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="586bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="586bd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="586bd-112">Parent elements</span></span>

[<span data-ttu-id="586bd-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="586bd-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="586bd-114">Text value</span><span class="sxs-lookup"><span data-stu-id="586bd-114">Text value</span></span>

<span data-ttu-id="586bd-115">Um valor de texto de **true** para o elemento **IsPermanentFailure** indica que uma tentativa anterior para indexar o item de caixa de correio foi bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="586bd-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="586bd-116">Um valor **false** indica que uma tentativa anterior para indexar o item de caixa de correio foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="586bd-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="586bd-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="586bd-117">Remarks</span></span>

<span data-ttu-id="586bd-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="586bd-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="586bd-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="586bd-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="586bd-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="586bd-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="586bd-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="586bd-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="586bd-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="586bd-122">Schema name</span></span>  <br/> |<span data-ttu-id="586bd-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="586bd-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="586bd-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="586bd-124">Validation file</span></span>  <br/> |<span data-ttu-id="586bd-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="586bd-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="586bd-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="586bd-126">Can be empty</span></span>  <br/> |<span data-ttu-id="586bd-127">false</span><span class="sxs-lookup"><span data-stu-id="586bd-127">false</span></span>  <br/> |
   

