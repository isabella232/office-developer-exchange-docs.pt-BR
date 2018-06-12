---
title: MarkAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkAsRead
api_type:
- schema
ms.assetid: 404842e1-fbdb-480d-a1d8-ba1ab2c9fb1e
description: O elemento MarkAsRead indica se as mensagens devem ser marcados como lidos.
ms.openlocfilehash: b453ad73912e99b6fd3aed84b03a7d2fc2b6a294
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824355"
---
# <a name="markasread"></a><span data-ttu-id="f8d44-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="f8d44-103">MarkAsRead</span></span>

<span data-ttu-id="f8d44-104">O elemento **MarkAsRead** indica se as mensagens devem ser marcados como lidos.</span><span class="sxs-lookup"><span data-stu-id="f8d44-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="f8d44-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f8d44-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8d44-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f8d44-106">Attributes and elements</span></span>

<span data-ttu-id="f8d44-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8d44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8d44-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8d44-108">Attributes</span></span>

<span data-ttu-id="f8d44-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8d44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8d44-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8d44-110">Child elements</span></span>

<span data-ttu-id="f8d44-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8d44-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8d44-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8d44-112">Parent elements</span></span>

|<span data-ttu-id="f8d44-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8d44-113">**Element**</span></span>|<span data-ttu-id="f8d44-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8d44-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8d44-115">Ações</span><span class="sxs-lookup"><span data-stu-id="f8d44-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="f8d44-116">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="f8d44-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f8d44-117">Text value</span><span class="sxs-lookup"><span data-stu-id="f8d44-117">Text value</span></span>

<span data-ttu-id="f8d44-118">Um valor de texto de **true** indica que a mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="f8d44-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="f8d44-119">Um valor **false** indica que as mensagens não devem ser marcadas como lidos.</span><span class="sxs-lookup"><span data-stu-id="f8d44-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f8d44-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8d44-120">Remarks</span></span>

<span data-ttu-id="f8d44-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8d44-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8d44-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f8d44-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8d44-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8d44-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8d44-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8d44-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f8d44-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f8d44-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8d44-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8d44-126">Validation File</span></span>  <br/> |<span data-ttu-id="f8d44-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f8d44-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8d44-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f8d44-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8d44-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f8d44-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8d44-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="f8d44-130">See also</span></span>



- [<span data-ttu-id="f8d44-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8d44-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

