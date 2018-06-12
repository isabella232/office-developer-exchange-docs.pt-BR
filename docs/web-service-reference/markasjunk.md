---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: O elemento MarkAsJunk Especifica a solicitação para mover um item para a pasta Lixo eletrônico e adicionar remetente à lista de remetentes bloqueados.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824350"
---
# <a name="markasjunk"></a><span data-ttu-id="da230-103">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="da230-103">MarkAsJunk</span></span>

<span data-ttu-id="da230-104">O elemento **MarkAsJunk** Especifica a solicitação para mover um item para a pasta Lixo eletrônico e adicionar remetente à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="da230-104">The **MarkAsJunk** element specifies the request to move an item to the junk mail folder and to add the sender to the blocked sender list.</span></span> 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 <span data-ttu-id="da230-105">**MarkAsJunkType**</span><span class="sxs-lookup"><span data-stu-id="da230-105">**MarkAsJunkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da230-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="da230-106">Attributes and elements</span></span>

<span data-ttu-id="da230-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="da230-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da230-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="da230-108">Attributes</span></span>

|<span data-ttu-id="da230-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="da230-109">**Attribute**</span></span>|<span data-ttu-id="da230-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="da230-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da230-111">IsJunk</span><span class="sxs-lookup"><span data-stu-id="da230-111">IsJunk</span></span>  <br/> |<span data-ttu-id="da230-112">Um valor de texto de **true** para o atributo **IsJunk** indica que o remetente do email é adicionado à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="da230-112">A text value of **true** for the **IsJunk** attribute indicates that the email sender is added to the blocked sender list.</span></span> <span data-ttu-id="da230-113">Um valor **false** indica que o remetente do email é removido da lista de remetentes bloqueados, se o remetente do email já estiver na lista.</span><span class="sxs-lookup"><span data-stu-id="da230-113">A value of **false** indicates that the email sender is removed from the blocked sender list, if the email sender is already on the list.</span></span>  <br/> |
|<span data-ttu-id="da230-114">MoveItem</span><span class="sxs-lookup"><span data-stu-id="da230-114">MoveItem</span></span>  <br/> |<span data-ttu-id="da230-115">Um valor de **true** para o atributo **MoveItem** text indica que o item é movido para a pasta de lixo eletrônico padrão.</span><span class="sxs-lookup"><span data-stu-id="da230-115">A text value of **true** for the **MoveItem** attribute indicates that the item is moved to the default junk mail folder.</span></span> <span data-ttu-id="da230-116">Um valor **false** indica que o item não será movido para a pasta de lixo eletrônico padrão.</span><span class="sxs-lookup"><span data-stu-id="da230-116">A value of **false** indicates that the item is not moved to the default junk mail folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="da230-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="da230-117">Child elements</span></span>

[<span data-ttu-id="da230-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="da230-118">ItemIds</span></span>](itemids.md)
  
### <a name="parent-elements"></a><span data-ttu-id="da230-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="da230-119">Parent elements</span></span>

<span data-ttu-id="da230-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="da230-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da230-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="da230-121">Remarks</span></span>

<span data-ttu-id="da230-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="da230-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="da230-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="da230-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da230-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="da230-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da230-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="da230-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da230-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="da230-126">Schema name</span></span>  <br/> |<span data-ttu-id="da230-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="da230-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da230-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="da230-128">Validation file</span></span>  <br/> |<span data-ttu-id="da230-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da230-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da230-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="da230-130">Can be empty</span></span>  <br/> ||
   

