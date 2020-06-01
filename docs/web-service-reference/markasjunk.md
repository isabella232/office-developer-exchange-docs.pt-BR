---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: O elemento MarkAsJunk especifica a solicitação para mover um item para a pasta lixo eletrônico e adicionar o remetente à lista de remetentes bloqueados.
ms.openlocfilehash: 99adc423864f3096772394ef290df20e158e457d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467078"
---
# <a name="markasjunk"></a><span data-ttu-id="d56bd-103">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="d56bd-103">MarkAsJunk</span></span>

<span data-ttu-id="d56bd-104">O elemento **MarkAsJunk** especifica a solicitação para mover um item para a pasta lixo eletrônico e adicionar o remetente à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d56bd-104">The **MarkAsJunk** element specifies the request to move an item to the junk mail folder and to add the sender to the blocked sender list.</span></span> 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 <span data-ttu-id="d56bd-105">**MarkAsJunkType**</span><span class="sxs-lookup"><span data-stu-id="d56bd-105">**MarkAsJunkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d56bd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d56bd-106">Attributes and elements</span></span>

<span data-ttu-id="d56bd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d56bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d56bd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d56bd-108">Attributes</span></span>

|<span data-ttu-id="d56bd-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d56bd-109">**Attribute**</span></span>|<span data-ttu-id="d56bd-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d56bd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d56bd-111">Islixo eletrônico</span><span class="sxs-lookup"><span data-stu-id="d56bd-111">IsJunk</span></span>  <br/> |<span data-ttu-id="d56bd-112">Um valor de texto **true** para o atributo **isjunk** indica que o remetente de email é adicionado à lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d56bd-112">A text value of **true** for the **IsJunk** attribute indicates that the email sender is added to the blocked sender list.</span></span> <span data-ttu-id="d56bd-113">Um valor **false** indica que o remetente de email será removido da lista de remetentes bloqueados, se o remetente de email já estiver na lista.</span><span class="sxs-lookup"><span data-stu-id="d56bd-113">A value of **false** indicates that the email sender is removed from the blocked sender list, if the email sender is already on the list.</span></span>  <br/> |
|<span data-ttu-id="d56bd-114">MoveItem</span><span class="sxs-lookup"><span data-stu-id="d56bd-114">MoveItem</span></span>  <br/> |<span data-ttu-id="d56bd-115">Um valor de texto **true** para o atributo **MoveItem** indica que o item é movido para a pasta de lixo eletrônico padrão.</span><span class="sxs-lookup"><span data-stu-id="d56bd-115">A text value of **true** for the **MoveItem** attribute indicates that the item is moved to the default junk mail folder.</span></span> <span data-ttu-id="d56bd-116">Um valor **false** indica que o item não é movido para a pasta de lixo eletrônico padrão.</span><span class="sxs-lookup"><span data-stu-id="d56bd-116">A value of **false** indicates that the item is not moved to the default junk mail folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d56bd-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d56bd-117">Child elements</span></span>

[<span data-ttu-id="d56bd-118">ItemIds</span><span class="sxs-lookup"><span data-stu-id="d56bd-118">ItemIds</span></span>](itemids.md)
  
### <a name="parent-elements"></a><span data-ttu-id="d56bd-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d56bd-119">Parent elements</span></span>

<span data-ttu-id="d56bd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d56bd-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d56bd-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="d56bd-121">Remarks</span></span>

<span data-ttu-id="d56bd-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d56bd-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d56bd-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d56bd-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d56bd-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d56bd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d56bd-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d56bd-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d56bd-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d56bd-126">Schema name</span></span>  <br/> |<span data-ttu-id="d56bd-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d56bd-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d56bd-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d56bd-128">Validation file</span></span>  <br/> |<span data-ttu-id="d56bd-129">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d56bd-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d56bd-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d56bd-130">Can be empty</span></span>  <br/> ||
   

