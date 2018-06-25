---
title: RedirectToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RedirectToRecipients
api_type:
- schema
ms.assetid: 00ef4a84-76d2-4669-b597-f52abbbc34f5
description: O elemento RedirectToRecipients indica os endereços de email para os quais as mensagens devem ser redirecionados.
ms.openlocfilehash: ca0422f2ca678cabe1a88f99e617bee691f2e2f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825024"
---
# <a name="redirecttorecipients"></a><span data-ttu-id="f589b-103">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="f589b-103">RedirectToRecipients</span></span>

<span data-ttu-id="f589b-104">O elemento **RedirectToRecipients** indica os endereços de email para os quais as mensagens devem ser redirecionados.</span><span class="sxs-lookup"><span data-stu-id="f589b-104">The **RedirectToRecipients** element indicates the e-mail addresses to which messages are to be redirected.</span></span> 
  
```XML
<RedirectToRecipients>
   <Address/>
</RedirectToRecipients>
```

 <span data-ttu-id="f589b-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="f589b-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f589b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f589b-106">Attributes and elements</span></span>

<span data-ttu-id="f589b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f589b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f589b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f589b-108">Attributes</span></span>

<span data-ttu-id="f589b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f589b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f589b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f589b-110">Child elements</span></span>

|<span data-ttu-id="f589b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f589b-111">**Element**</span></span>|<span data-ttu-id="f589b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f589b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f589b-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f589b-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="f589b-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="f589b-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f589b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f589b-115">Parent elements</span></span>

|<span data-ttu-id="f589b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f589b-116">**Element**</span></span>|<span data-ttu-id="f589b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f589b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f589b-118">Ações</span><span class="sxs-lookup"><span data-stu-id="f589b-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="f589b-119">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="f589b-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f589b-120">Text value</span><span class="sxs-lookup"><span data-stu-id="f589b-120">Text value</span></span>

<span data-ttu-id="f589b-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f589b-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f589b-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="f589b-122">Remarks</span></span>

<span data-ttu-id="f589b-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f589b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f589b-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f589b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f589b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="f589b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f589b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f589b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f589b-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f589b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f589b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f589b-128">Validation File</span></span>  <br/> |<span data-ttu-id="f589b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f589b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f589b-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f589b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f589b-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f589b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f589b-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="f589b-132">See also</span></span>



- [<span data-ttu-id="f589b-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f589b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

