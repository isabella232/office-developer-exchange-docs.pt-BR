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
description: O elemento RedirectToRecipients indica os endereços de email aos quais as mensagens devem ser redirecionadas.
ms.openlocfilehash: ebc0e0abe88d1e364dee94cc24313879458778d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462189"
---
# <a name="redirecttorecipients"></a><span data-ttu-id="939b2-103">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="939b2-103">RedirectToRecipients</span></span>

<span data-ttu-id="939b2-104">O elemento **RedirectToRecipients** indica os endereços de email aos quais as mensagens devem ser redirecionadas.</span><span class="sxs-lookup"><span data-stu-id="939b2-104">The **RedirectToRecipients** element indicates the e-mail addresses to which messages are to be redirected.</span></span> 
  
```XML
<RedirectToRecipients>
   <Address/>
</RedirectToRecipients>
```

 <span data-ttu-id="939b2-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="939b2-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="939b2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="939b2-106">Attributes and elements</span></span>

<span data-ttu-id="939b2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="939b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="939b2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="939b2-108">Attributes</span></span>

<span data-ttu-id="939b2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="939b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="939b2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="939b2-110">Child elements</span></span>

|<span data-ttu-id="939b2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="939b2-111">**Element**</span></span>|<span data-ttu-id="939b2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="939b2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="939b2-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="939b2-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="939b2-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="939b2-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="939b2-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="939b2-115">Parent elements</span></span>

|<span data-ttu-id="939b2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="939b2-116">**Element**</span></span>|<span data-ttu-id="939b2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="939b2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="939b2-118">Actions</span><span class="sxs-lookup"><span data-stu-id="939b2-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="939b2-119">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="939b2-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="939b2-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="939b2-120">Text value</span></span>

<span data-ttu-id="939b2-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="939b2-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="939b2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="939b2-122">Remarks</span></span>

<span data-ttu-id="939b2-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="939b2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="939b2-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="939b2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="939b2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="939b2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="939b2-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="939b2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="939b2-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="939b2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="939b2-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="939b2-128">Validation File</span></span>  <br/> |<span data-ttu-id="939b2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="939b2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="939b2-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="939b2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="939b2-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="939b2-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="939b2-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="939b2-132">See also</span></span>



- [<span data-ttu-id="939b2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="939b2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

