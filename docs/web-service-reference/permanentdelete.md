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
description: O elemento PermanentDelete indica se as mensagens devem ser excluídos permanentemente e não são salvas na pasta Itens excluídos.
ms.openlocfilehash: 40cf80e054bb70a3f6d687e8d4361f1d4331a7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824724"
---
# <a name="permanentdelete"></a><span data-ttu-id="e7d98-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="e7d98-103">PermanentDelete</span></span>

<span data-ttu-id="e7d98-104">O elemento **PermanentDelete** indica se as mensagens devem ser excluídos permanentemente e não são salvas na pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e7d98-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="e7d98-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e7d98-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7d98-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e7d98-106">Attributes and elements</span></span>

<span data-ttu-id="e7d98-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7d98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7d98-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7d98-108">Attributes</span></span>

<span data-ttu-id="e7d98-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7d98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7d98-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7d98-110">Child elements</span></span>

<span data-ttu-id="e7d98-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7d98-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7d98-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7d98-112">Parent elements</span></span>

|<span data-ttu-id="e7d98-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7d98-113">**Element**</span></span>|<span data-ttu-id="e7d98-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7d98-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7d98-115">Ações</span><span class="sxs-lookup"><span data-stu-id="e7d98-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="e7d98-116">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="e7d98-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7d98-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e7d98-117">Text value</span></span>

<span data-ttu-id="e7d98-118">Um valor de texto de **true** indica que a mensagem deve ser marcada para ser excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="e7d98-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="e7d98-119">Um valor **false** indica que a mensagem não deve ser marcada para ser excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="e7d98-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e7d98-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e7d98-120">Remarks</span></span>

<span data-ttu-id="e7d98-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7d98-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7d98-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e7d98-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7d98-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7d98-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7d98-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7d98-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e7d98-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e7d98-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e7d98-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7d98-126">Validation File</span></span>  <br/> |<span data-ttu-id="e7d98-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e7d98-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7d98-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e7d98-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7d98-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e7d98-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7d98-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="e7d98-130">See also</span></span>



- [<span data-ttu-id="e7d98-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7d98-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

