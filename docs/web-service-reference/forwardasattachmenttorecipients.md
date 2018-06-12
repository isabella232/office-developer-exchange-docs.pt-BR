---
title: ForwardAsAttachmentToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardAsAttachmentToRecipients
api_type:
- schema
ms.assetid: 8649ea14-672f-43c9-b10a-a2b02efd5867
description: O elemento ForwardAsAttachmentToRecipients indica os endereços de email ao qual as mensagens devem ser encaminhadas como anexos.
ms.openlocfilehash: 04d4f9c6228e6d0ab34a6eff5d5751f461a57e19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752351"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="c0a8e-103">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="c0a8e-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="c0a8e-104">O elemento **ForwardAsAttachmentToRecipients** indica os endereços de email ao qual as mensagens devem ser encaminhadas como anexos.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="c0a8e-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="c0a8e-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0a8e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c0a8e-106">Attributes and elements</span></span>

<span data-ttu-id="c0a8e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0a8e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0a8e-108">Attributes</span></span>

<span data-ttu-id="c0a8e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0a8e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0a8e-110">Child elements</span></span>

|<span data-ttu-id="c0a8e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0a8e-111">**Element**</span></span>|<span data-ttu-id="c0a8e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0a8e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0a8e-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="c0a8e-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="c0a8e-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0a8e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0a8e-115">Parent elements</span></span>

|<span data-ttu-id="c0a8e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0a8e-116">**Element**</span></span>|<span data-ttu-id="c0a8e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0a8e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0a8e-118">Ações</span><span class="sxs-lookup"><span data-stu-id="c0a8e-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c0a8e-119">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0a8e-120">Text value</span><span class="sxs-lookup"><span data-stu-id="c0a8e-120">Text value</span></span>

<span data-ttu-id="c0a8e-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0a8e-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0a8e-122">Remarks</span></span>

<span data-ttu-id="c0a8e-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0a8e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0a8e-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c0a8e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0a8e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0a8e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c0a8e-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0a8e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c0a8e-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c0a8e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c0a8e-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0a8e-128">Validation File</span></span>  <br/> |<span data-ttu-id="c0a8e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0a8e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0a8e-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c0a8e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0a8e-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c0a8e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0a8e-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="c0a8e-132">See also</span></span>



- [<span data-ttu-id="c0a8e-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c0a8e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

