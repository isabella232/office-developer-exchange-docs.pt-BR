---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: O elemento ReadFlag indica o estado de leitura para definir em itens em uma pasta.
ms.openlocfilehash: f3156a51fbdd3372dd28f2065499d26a50b3d497
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824954"
---
# <a name="readflag"></a><span data-ttu-id="1399b-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="1399b-103">ReadFlag</span></span>

<span data-ttu-id="1399b-104">O elemento **ReadFlag** indica o estado de leitura para definir em itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="1399b-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="1399b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1399b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1399b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1399b-106">Attributes and elements</span></span>

<span data-ttu-id="1399b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1399b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1399b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1399b-108">Attributes</span></span>

<span data-ttu-id="1399b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1399b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1399b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1399b-110">Child elements</span></span>

<span data-ttu-id="1399b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1399b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1399b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1399b-112">Parent elements</span></span>

[<span data-ttu-id="1399b-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="1399b-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="1399b-114">Text value</span><span class="sxs-lookup"><span data-stu-id="1399b-114">Text value</span></span>

<span data-ttu-id="1399b-115">Um valor de texto de **true** para o elemento **ReadFlag** indica que os itens na pasta serão marcados como lida.</span><span class="sxs-lookup"><span data-stu-id="1399b-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="1399b-116">Um valor **false** indica que os itens na pasta serão marcados como não lido.</span><span class="sxs-lookup"><span data-stu-id="1399b-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1399b-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="1399b-117">Remarks</span></span>

<span data-ttu-id="1399b-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1399b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1399b-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1399b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1399b-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1399b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1399b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="1399b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1399b-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1399b-122">Schema name</span></span>  <br/> |<span data-ttu-id="1399b-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1399b-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1399b-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1399b-124">Validation file</span></span>  <br/> |<span data-ttu-id="1399b-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1399b-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1399b-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1399b-126">Can be empty</span></span>  <br/> ||
   

