---
title: MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22244afb-99ec-41b4-8f73-3fbccd56d1ab
description: O elemento MarkAllItemsAsRead contém a solicitação para marcar todos os itens de uma pasta como lidos.
ms.openlocfilehash: 0338b2a1eed503b7e8fb0ec8b4a8ebcf12b6dbd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530885"
---
# <a name="markallitemsasread"></a><span data-ttu-id="972db-103">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="972db-103">MarkAllItemsAsRead</span></span>

<span data-ttu-id="972db-104">O elemento **MarkAllItemsAsRead** contém a solicitação para marcar todos os itens de uma pasta como lidos.</span><span class="sxs-lookup"><span data-stu-id="972db-104">The **MarkAllItemsAsRead** element contains the request to mark all the items in a folder as read.</span></span> 
  
```XML
<MarkAllItemsAsRead>
   <ReadFlag/>
   <SuppressReadReceipts/>
   <FolderIds/>
</MarkAllItemsAsRead>
```

 <span data-ttu-id="972db-105">**MarkAllItemsAsReadType**</span><span class="sxs-lookup"><span data-stu-id="972db-105">**MarkAllItemsAsReadType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="972db-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="972db-106">Attributes and elements</span></span>

<span data-ttu-id="972db-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="972db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="972db-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="972db-108">Attributes</span></span>

<span data-ttu-id="972db-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="972db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="972db-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="972db-110">Child elements</span></span>

<span data-ttu-id="972db-111">[ReadFlag](readflag.md)  |  [SuppressReadReceipts](suppressreadreceipts.md)  |  [FolderIds](folderids.md)</span><span class="sxs-lookup"><span data-stu-id="972db-111">[ReadFlag](readflag.md) | [SuppressReadReceipts](suppressreadreceipts.md) | [FolderIds](folderids.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="972db-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="972db-112">Parent elements</span></span>

<span data-ttu-id="972db-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="972db-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="972db-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="972db-114">Remarks</span></span>

<span data-ttu-id="972db-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="972db-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="972db-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="972db-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="972db-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="972db-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="972db-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="972db-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="972db-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="972db-119">Schema name</span></span>  <br/> |<span data-ttu-id="972db-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="972db-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="972db-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="972db-121">Validation file</span></span>  <br/> |<span data-ttu-id="972db-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="972db-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="972db-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="972db-123">Can be empty</span></span>  <br/> ||
   

