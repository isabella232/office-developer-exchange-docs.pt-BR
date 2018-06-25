---
title: ForwardToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardToRecipients
api_type:
- schema
ms.assetid: dd58fd72-591d-4891-b226-465bcf12c19b
description: O elemento ForwardToRecipients indica os endereços de email ao qual as mensagens devem ser encaminhadas.
ms.openlocfilehash: f2538f62bb9d837ef64bdc742b01d26d3d7d77f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752353"
---
# <a name="forwardtorecipients"></a><span data-ttu-id="c2f39-103">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="c2f39-103">ForwardToRecipients</span></span>

<span data-ttu-id="c2f39-104">O elemento **ForwardToRecipients** indica os endereços de email ao qual as mensagens devem ser encaminhadas.</span><span class="sxs-lookup"><span data-stu-id="c2f39-104">The **ForwardToRecipients** element indicates the e-mail addresses to which messages are to be forwarded.</span></span> 
  
```XML
<ForwardToRecipients>
   <Address/>
</ForwardToRecipients>
```

 <span data-ttu-id="c2f39-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="c2f39-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2f39-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2f39-106">Attributes and elements</span></span>

<span data-ttu-id="c2f39-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2f39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2f39-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2f39-108">Attributes</span></span>

<span data-ttu-id="c2f39-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2f39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2f39-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2f39-110">Child elements</span></span>

|<span data-ttu-id="c2f39-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2f39-111">**Element**</span></span>|<span data-ttu-id="c2f39-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2f39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2f39-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c2f39-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="c2f39-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="c2f39-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2f39-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2f39-115">Parent elements</span></span>

|<span data-ttu-id="c2f39-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2f39-116">**Element**</span></span>|<span data-ttu-id="c2f39-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2f39-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2f39-118">Ações</span><span class="sxs-lookup"><span data-stu-id="c2f39-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c2f39-119">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="c2f39-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2f39-120">Text value</span><span class="sxs-lookup"><span data-stu-id="c2f39-120">Text value</span></span>

<span data-ttu-id="c2f39-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2f39-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2f39-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2f39-122">Remarks</span></span>

<span data-ttu-id="c2f39-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2f39-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2f39-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2f39-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2f39-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2f39-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2f39-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2f39-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c2f39-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c2f39-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2f39-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2f39-128">Validation File</span></span>  <br/> |<span data-ttu-id="c2f39-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2f39-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2f39-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2f39-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2f39-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c2f39-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2f39-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="c2f39-132">See also</span></span>



- [<span data-ttu-id="c2f39-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c2f39-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

