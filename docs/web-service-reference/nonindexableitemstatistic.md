---
title: NonIndexableItemStatistic
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 593e0c79-9ec2-4040-a6a3-3c5c61cbdf7c
description: O elemento NonIndexableItemStatistic contém uma única estatística para um item que não pôde ser indexado
ms.openlocfilehash: cc7bee9fd2759a16dd16538d6712e40ceb005fec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462679"
---
# <a name="nonindexableitemstatistic"></a><span data-ttu-id="c01b5-103">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="c01b5-103">NonIndexableItemStatistic</span></span>

<span data-ttu-id="c01b5-104">O elemento **NonIndexableItemStatistic** contém uma única estatística para um item que não pôde ser indexado</span><span class="sxs-lookup"><span data-stu-id="c01b5-104">The **NonIndexableItemStatistic** element contains a single statistic for an item that could not be indexed</span></span> 
  
```XML
<NonIndexableItemStatistic>
   <Mailbox/>
   <ItemCount/>
   <ErrorMessage/>
</NonIndexableItemStatistic>
```

 <span data-ttu-id="c01b5-105">**NonIndexableItemStatisticType**</span><span class="sxs-lookup"><span data-stu-id="c01b5-105">**NonIndexableItemStatisticType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c01b5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c01b5-106">Attributes and elements</span></span>

<span data-ttu-id="c01b5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c01b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c01b5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c01b5-108">Attributes</span></span>

<span data-ttu-id="c01b5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c01b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c01b5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c01b5-110">Child elements</span></span>

<span data-ttu-id="c01b5-111">[Caixa de correio (cadeia de caracteres)](mailbox-string.md)  |  [ItemCount](itemcount.md)  |  [ErrorMessage](errormessage.md)</span><span class="sxs-lookup"><span data-stu-id="c01b5-111">[Mailbox (string)](mailbox-string.md) | [ItemCount](itemcount.md) | [ErrorMessage](errormessage.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c01b5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c01b5-112">Parent elements</span></span>

[<span data-ttu-id="c01b5-113">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="c01b5-113">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
  
## <a name="remarks"></a><span data-ttu-id="c01b5-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="c01b5-114">Remarks</span></span>

<span data-ttu-id="c01b5-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c01b5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c01b5-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c01b5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c01b5-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c01b5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c01b5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c01b5-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c01b5-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c01b5-119">Schema name</span></span>  <br/> |<span data-ttu-id="c01b5-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c01b5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c01b5-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c01b5-121">Validation file</span></span>  <br/> |<span data-ttu-id="c01b5-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c01b5-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c01b5-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c01b5-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c01b5-124">False</span><span class="sxs-lookup"><span data-stu-id="c01b5-124">False</span></span>  <br/> |
   

