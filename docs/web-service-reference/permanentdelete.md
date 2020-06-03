---
title: PermanentDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: O elemento PermanentDelete indica se as mensagens devem ser excluídas permanentemente e não foram salvas na pasta itens excluídos.
ms.openlocfilehash: da7680eefca9ad359948af38eac49d18e9055988
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467764"
---
# <a name="permanentdelete"></a><span data-ttu-id="1b05d-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="1b05d-103">PermanentDelete</span></span>

<span data-ttu-id="1b05d-104">O elemento **PermanentDelete** indica se as mensagens devem ser excluídas permanentemente e não foram salvas na pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="1b05d-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="1b05d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1b05d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b05d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1b05d-106">Attributes and elements</span></span>

<span data-ttu-id="1b05d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1b05d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b05d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1b05d-108">Attributes</span></span>

<span data-ttu-id="1b05d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b05d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b05d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1b05d-110">Child elements</span></span>

<span data-ttu-id="1b05d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b05d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b05d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1b05d-112">Parent elements</span></span>

|<span data-ttu-id="1b05d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b05d-113">**Element**</span></span>|<span data-ttu-id="1b05d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b05d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b05d-115">Actions</span><span class="sxs-lookup"><span data-stu-id="1b05d-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="1b05d-116">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="1b05d-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b05d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1b05d-117">Text value</span></span>

<span data-ttu-id="1b05d-118">Um valor de texto **true** indica que a mensagem deve ser marcada para ser excluída permanentemente.</span><span class="sxs-lookup"><span data-stu-id="1b05d-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="1b05d-119">Um valor **false** indica que a mensagem não deve ser marcada para ser excluída permanentemente.</span><span class="sxs-lookup"><span data-stu-id="1b05d-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1b05d-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1b05d-120">Remarks</span></span>

<span data-ttu-id="1b05d-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b05d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b05d-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1b05d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b05d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1b05d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b05d-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1b05d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1b05d-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1b05d-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b05d-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1b05d-126">Validation File</span></span>  <br/> |<span data-ttu-id="1b05d-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b05d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b05d-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1b05d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b05d-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="1b05d-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b05d-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="1b05d-130">See also</span></span>



- [<span data-ttu-id="1b05d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1b05d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

