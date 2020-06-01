---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: O elemento SuppressReadReceipts indica se as confirmações de leitura devem ser suprimidas.
ms.openlocfilehash: aa604d4907582bd73727ba664958a589a222f9cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455930"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="5425a-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="5425a-103">SuppressReadReceipts</span></span>

<span data-ttu-id="5425a-104">O elemento **SuppressReadReceipts** indica se as confirmações de leitura devem ser suprimidas.</span><span class="sxs-lookup"><span data-stu-id="5425a-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="5425a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5425a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5425a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5425a-106">Attributes and elements</span></span>

<span data-ttu-id="5425a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5425a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5425a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5425a-108">Attributes</span></span>

<span data-ttu-id="5425a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5425a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5425a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5425a-110">Child elements</span></span>

<span data-ttu-id="5425a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5425a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5425a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5425a-112">Parent elements</span></span>

<span data-ttu-id="5425a-113">[Conversation](conversationaction.md)  |  [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="5425a-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5425a-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5425a-114">Text value</span></span>

<span data-ttu-id="5425a-115">Um valor de texto **true** para o elemento **SuppressReadReciepts** indica que as confirmações de leitura são suprimidas.</span><span class="sxs-lookup"><span data-stu-id="5425a-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="5425a-116">Um valor **false** indica que as confirmações de leitura serão enviadas ao remetente.</span><span class="sxs-lookup"><span data-stu-id="5425a-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5425a-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="5425a-117">Remarks</span></span>

<span data-ttu-id="5425a-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5425a-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5425a-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5425a-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5425a-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5425a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5425a-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5425a-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5425a-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5425a-122">Schema name</span></span>  <br/> |<span data-ttu-id="5425a-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5425a-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5425a-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5425a-124">Validation file</span></span>  <br/> |<span data-ttu-id="5425a-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5425a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5425a-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5425a-126">Can be empty</span></span>  <br/> ||
   

