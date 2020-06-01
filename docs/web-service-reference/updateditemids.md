---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: O elemento UpdatedItemIds especifica os identificadores dos itens de lembrete atualizados.
ms.openlocfilehash: 4a87bf50f90e80c0c887ee3a66b9f201ea1c8440
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465033"
---
# <a name="updateditemids"></a><span data-ttu-id="b74af-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="b74af-103">UpdatedItemIds</span></span>

<span data-ttu-id="b74af-104">O elemento **UpdatedItemIds** especifica os identificadores dos itens de lembrete atualizados.</span><span class="sxs-lookup"><span data-stu-id="b74af-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="b74af-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="b74af-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b74af-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b74af-106">Attributes and elements</span></span>

<span data-ttu-id="b74af-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b74af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b74af-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b74af-108">Attributes</span></span>

<span data-ttu-id="b74af-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b74af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b74af-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b74af-110">Child elements</span></span>

[<span data-ttu-id="b74af-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="b74af-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="b74af-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b74af-112">Parent elements</span></span>

[<span data-ttu-id="b74af-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b74af-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="b74af-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="b74af-114">Remarks</span></span>

<span data-ttu-id="b74af-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b74af-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b74af-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b74af-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="b74af-117">Se a operação [PerformReminderAction](performreminderaction-operation.md) não for concluída com êxito ou se nenhuma alteração tiver sido feita no servidor, o elemento **UpdatedItemIds** será retornado como um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="b74af-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b74af-118">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b74af-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b74af-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="b74af-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b74af-120">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b74af-120">Schema Name</span></span>  <br/> |<span data-ttu-id="b74af-121">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b74af-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b74af-122">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b74af-122">Validation File</span></span>  <br/> |<span data-ttu-id="b74af-123">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b74af-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b74af-124">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b74af-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="b74af-125">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b74af-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b74af-126">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b74af-126">See also</span></span>



[<span data-ttu-id="b74af-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b74af-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="b74af-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b74af-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

