---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: O elemento MarkAllItemsAsRead contém a solicitação para marcar todos os itens em uma pasta como lidos.
ms.openlocfilehash: 9d7eb8eb7194cb5d77e909dc08abfb70e2385d56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824346"
---
# <a name="markallitemsasread"></a><span data-ttu-id="91cca-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="91cca-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="91cca-104">O elemento **MarkAllItemsAsRead** contém a solicitação para marcar todos os itens em uma pasta como lidos.</span><span class="sxs-lookup"><span data-stu-id="91cca-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="91cca-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="91cca-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91cca-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="91cca-106">Attributes and elements</span></span>

<span data-ttu-id="91cca-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91cca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91cca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91cca-108">Attributes</span></span>

<span data-ttu-id="91cca-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91cca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91cca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91cca-110">Child elements</span></span>

<span data-ttu-id="91cca-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="91cca-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91cca-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91cca-112">Parent elements</span></span>

<span data-ttu-id="91cca-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91cca-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91cca-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="91cca-114">Remarks</span></span>

<span data-ttu-id="91cca-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91cca-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91cca-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91cca-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91cca-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="91cca-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91cca-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="91cca-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="91cca-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91cca-119">Schema name</span></span>  <br/> |<span data-ttu-id="91cca-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="91cca-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="91cca-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91cca-121">Validation file</span></span>  <br/> |<span data-ttu-id="91cca-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="91cca-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="91cca-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="91cca-123">Can be empty</span></span>  <br/> ||
   

