---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: O elemento UpdateItemInRecoverableItems especifica uma solicitação para atualizar um item em itens recuperáveis.
ms.openlocfilehash: f3dae55097c613b84a80795185baad559e312b90
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459781"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="ff9ea-103">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="ff9ea-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="ff9ea-104">O elemento **UpdateItemInRecoverableItems** especifica uma solicitação para atualizar um item em itens recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="ff9ea-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="ff9ea-105">**UpdateItemInRecoverableItemsType**</span><span class="sxs-lookup"><span data-stu-id="ff9ea-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff9ea-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ff9ea-106">Attributes and elements</span></span>

<span data-ttu-id="ff9ea-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ff9ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff9ea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ff9ea-108">Attributes</span></span>

<span data-ttu-id="ff9ea-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff9ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff9ea-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ff9ea-110">Child elements</span></span>

<span data-ttu-id="ff9ea-111">[ItemId](itemid.md)  |  [Atualizações (item)](updates-item.md)  |  [Anexos](attachments-ex15websvcsotherref.md)  |  [MakeItemImmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="ff9ea-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff9ea-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ff9ea-112">Parent elements</span></span>

<span data-ttu-id="ff9ea-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff9ea-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff9ea-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="ff9ea-114">Remarks</span></span>

<span data-ttu-id="ff9ea-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff9ea-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff9ea-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff9ea-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff9ea-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ff9ea-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff9ea-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff9ea-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff9ea-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ff9ea-119">Schema name</span></span>  <br/> |<span data-ttu-id="ff9ea-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ff9ea-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff9ea-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ff9ea-121">Validation file</span></span>  <br/> |<span data-ttu-id="ff9ea-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff9ea-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff9ea-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ff9ea-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ff9ea-124">falso</span><span class="sxs-lookup"><span data-stu-id="ff9ea-124">false</span></span>  <br/> |
   

