---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: O elemento indica se a notificação de leitura de SuppressReadReceipts deve ser suprimida.
ms.openlocfilehash: 794252da6b3e6b6e6f36181c1811a2a001bfaf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837678"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="3dd20-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="3dd20-103">SuppressReadReceipts</span></span>

<span data-ttu-id="3dd20-104">O elemento **SuppressReadReceipts** indica se ler confirmações devem ser suprimidas.</span><span class="sxs-lookup"><span data-stu-id="3dd20-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="3dd20-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3dd20-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dd20-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3dd20-106">Attributes and elements</span></span>

<span data-ttu-id="3dd20-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3dd20-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dd20-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3dd20-108">Attributes</span></span>

<span data-ttu-id="3dd20-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dd20-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dd20-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3dd20-110">Child elements</span></span>

<span data-ttu-id="3dd20-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dd20-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3dd20-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3dd20-112">Parent elements</span></span>

<span data-ttu-id="3dd20-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="3dd20-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3dd20-114">Text value</span><span class="sxs-lookup"><span data-stu-id="3dd20-114">Text value</span></span>

<span data-ttu-id="3dd20-115">Um valor de texto de **true** para o elemento **SuppressReadReciepts** indica read confirmações são suprimidas.</span><span class="sxs-lookup"><span data-stu-id="3dd20-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="3dd20-116">Um valor **false** indica que são lidas confirmações serão enviadas ao remetente.</span><span class="sxs-lookup"><span data-stu-id="3dd20-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3dd20-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3dd20-117">Remarks</span></span>

<span data-ttu-id="3dd20-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3dd20-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3dd20-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3dd20-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dd20-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3dd20-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dd20-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dd20-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3dd20-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3dd20-122">Schema name</span></span>  <br/> |<span data-ttu-id="3dd20-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3dd20-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3dd20-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3dd20-124">Validation file</span></span>  <br/> |<span data-ttu-id="3dd20-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3dd20-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dd20-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3dd20-126">Can be empty</span></span>  <br/> ||
   

