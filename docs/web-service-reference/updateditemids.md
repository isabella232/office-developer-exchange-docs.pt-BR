---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: O elemento UpdatedItemIds Especifica os identificadores dos itens de lembrete atualizados.
ms.openlocfilehash: b95ebb20823706e68b1fd66dc64f756808bb7375
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837883"
---
# <a name="updateditemids"></a><span data-ttu-id="32d31-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="32d31-103">UpdatedItemIds</span></span>

<span data-ttu-id="32d31-104">O elemento **UpdatedItemIds** Especifica os identificadores dos itens de lembrete atualizados.</span><span class="sxs-lookup"><span data-stu-id="32d31-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="32d31-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="32d31-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32d31-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="32d31-106">Attributes and elements</span></span>

<span data-ttu-id="32d31-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="32d31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32d31-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="32d31-108">Attributes</span></span>

<span data-ttu-id="32d31-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32d31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32d31-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="32d31-110">Child elements</span></span>

[<span data-ttu-id="32d31-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="32d31-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="32d31-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="32d31-112">Parent elements</span></span>

[<span data-ttu-id="32d31-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="32d31-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="32d31-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="32d31-114">Remarks</span></span>

<span data-ttu-id="32d31-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="32d31-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="32d31-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="32d31-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="32d31-117">Se a operação [PerformReminderAction](performreminderaction-operation.md) não foi concluída com êxito ou não foram feitas alterações no servidor, o elemento **UpdatedItemIds** é retornado como um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="32d31-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="32d31-118">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="32d31-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32d31-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="32d31-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32d31-120">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="32d31-120">Schema Name</span></span>  <br/> |<span data-ttu-id="32d31-121">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="32d31-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32d31-122">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="32d31-122">Validation File</span></span>  <br/> |<span data-ttu-id="32d31-123">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32d31-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32d31-124">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="32d31-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="32d31-125">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="32d31-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32d31-126">Ver também</span><span class="sxs-lookup"><span data-stu-id="32d31-126">See also</span></span>



[<span data-ttu-id="32d31-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="32d31-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="32d31-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="32d31-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

