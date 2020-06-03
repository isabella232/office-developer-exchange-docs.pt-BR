---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: O elemento ReadFlag indica o estado de leitura a ser definido em itens em uma pasta.
ms.openlocfilehash: 1d3b9f3fe199ed2e63bdb632135120a5f89f4d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529893"
---
# <a name="readflag"></a><span data-ttu-id="ceff5-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="ceff5-103">ReadFlag</span></span>

<span data-ttu-id="ceff5-104">O elemento **ReadFlag** indica o estado de leitura a ser definido em itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ceff5-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="ceff5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ceff5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ceff5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ceff5-106">Attributes and elements</span></span>

<span data-ttu-id="ceff5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ceff5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ceff5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ceff5-108">Attributes</span></span>

<span data-ttu-id="ceff5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ceff5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ceff5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ceff5-110">Child elements</span></span>

<span data-ttu-id="ceff5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ceff5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ceff5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ceff5-112">Parent elements</span></span>

[<span data-ttu-id="ceff5-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="ceff5-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="ceff5-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ceff5-114">Text value</span></span>

<span data-ttu-id="ceff5-115">Um valor de texto **true** para o elemento **ReadFlag** indica que os itens na pasta serão marcados como lidos.</span><span class="sxs-lookup"><span data-stu-id="ceff5-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="ceff5-116">Um valor **false** indica que os itens na pasta serão marcados como não lidos.</span><span class="sxs-lookup"><span data-stu-id="ceff5-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ceff5-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="ceff5-117">Remarks</span></span>

<span data-ttu-id="ceff5-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ceff5-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ceff5-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ceff5-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ceff5-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ceff5-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ceff5-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="ceff5-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ceff5-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ceff5-122">Schema name</span></span>  <br/> |<span data-ttu-id="ceff5-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ceff5-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ceff5-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ceff5-124">Validation file</span></span>  <br/> |<span data-ttu-id="ceff5-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ceff5-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ceff5-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ceff5-126">Can be empty</span></span>  <br/> ||
   

