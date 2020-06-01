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
description: O elemento ForwardAsAttachmentToRecipients indica os endereços de email para os quais as mensagens devem ser encaminhadas como anexos.
ms.openlocfilehash: bf8c3563460eea811602074bf16f9253b4610832
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44453333"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="d9414-103">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="d9414-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="d9414-104">O elemento **ForwardAsAttachmentToRecipients** indica os endereços de email para os quais as mensagens devem ser encaminhadas como anexos.</span><span class="sxs-lookup"><span data-stu-id="d9414-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="d9414-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="d9414-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9414-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d9414-106">Attributes and elements</span></span>

<span data-ttu-id="d9414-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9414-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9414-108">Attributes</span></span>

<span data-ttu-id="d9414-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9414-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9414-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9414-110">Child elements</span></span>

|<span data-ttu-id="d9414-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9414-111">**Element**</span></span>|<span data-ttu-id="d9414-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9414-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9414-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d9414-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="d9414-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d9414-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9414-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9414-115">Parent elements</span></span>

|<span data-ttu-id="d9414-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9414-116">**Element**</span></span>|<span data-ttu-id="d9414-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9414-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9414-118">Actions</span><span class="sxs-lookup"><span data-stu-id="d9414-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="d9414-119">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="d9414-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9414-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d9414-120">Text value</span></span>

<span data-ttu-id="d9414-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9414-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9414-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9414-122">Remarks</span></span>

<span data-ttu-id="d9414-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9414-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9414-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d9414-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9414-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9414-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d9414-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9414-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d9414-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d9414-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d9414-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9414-128">Validation File</span></span>  <br/> |<span data-ttu-id="d9414-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d9414-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d9414-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9414-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9414-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d9414-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9414-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d9414-132">See also</span></span>



- [<span data-ttu-id="d9414-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9414-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

