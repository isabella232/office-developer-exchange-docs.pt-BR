---
title: SendSMSAlertToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendSMSAlertToRecipients
api_type:
- schema
ms.assetid: c4dd000b-11b6-4b7b-91e0-dbfeae11d770
description: O elemento SendSMSAlertToRecipients indica os números de telefone celular para o qual um alerta do serviço SMS (Short Message) será enviado.
ms.openlocfilehash: b28202c71257fccca67879713d5d7df03f69b06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825347"
---
# <a name="sendsmsalerttorecipients"></a><span data-ttu-id="1b5f3-103">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="1b5f3-103">SendSMSAlertToRecipients</span></span>

<span data-ttu-id="1b5f3-104">O elemento **SendSMSAlertToRecipients** indica os números de telefone celular para o qual um alerta do serviço SMS (Short Message) será enviado.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-104">The **SendSMSAlertToRecipients** element indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span> 
  
```XML
<SendSMSAlertToRecipients>
   <Address/>
</SendSMSAlertToRecipients>
```

 <span data-ttu-id="1b5f3-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="1b5f3-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b5f3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1b5f3-106">Attributes and elements</span></span>

<span data-ttu-id="1b5f3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b5f3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1b5f3-108">Attributes</span></span>

<span data-ttu-id="1b5f3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b5f3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1b5f3-110">Child elements</span></span>

|<span data-ttu-id="1b5f3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b5f3-111">**Element**</span></span>|<span data-ttu-id="1b5f3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b5f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b5f3-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1b5f3-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="1b5f3-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b5f3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1b5f3-115">Parent elements</span></span>

|<span data-ttu-id="1b5f3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b5f3-116">**Element**</span></span>|<span data-ttu-id="1b5f3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b5f3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b5f3-118">Ações</span><span class="sxs-lookup"><span data-stu-id="1b5f3-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="1b5f3-119">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b5f3-120">Text value</span><span class="sxs-lookup"><span data-stu-id="1b5f3-120">Text value</span></span>

<span data-ttu-id="1b5f3-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b5f3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="1b5f3-122">Remarks</span></span>

<span data-ttu-id="1b5f3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b5f3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b5f3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1b5f3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b5f3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1b5f3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b5f3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1b5f3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1b5f3-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1b5f3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b5f3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1b5f3-128">Validation File</span></span>  <br/> |<span data-ttu-id="1b5f3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b5f3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b5f3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1b5f3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b5f3-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="1b5f3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b5f3-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="1b5f3-132">See also</span></span>



- [<span data-ttu-id="1b5f3-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1b5f3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

