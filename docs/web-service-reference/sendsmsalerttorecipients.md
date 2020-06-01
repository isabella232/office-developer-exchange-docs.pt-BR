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
description: O elemento SendSMSAlertToRecipients indica os números de telefone celular para os quais um alerta de serviço de mensagem curta (SMS) deve ser enviado.
ms.openlocfilehash: ed17bf9ad20a51cbead4b86f385a53d19562fa64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464844"
---
# <a name="sendsmsalerttorecipients"></a><span data-ttu-id="d4839-103">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="d4839-103">SendSMSAlertToRecipients</span></span>

<span data-ttu-id="d4839-104">O elemento **SendSMSAlertToRecipients** indica os números de telefone celular para os quais um alerta de serviço de mensagem curta (SMS) deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="d4839-104">The **SendSMSAlertToRecipients** element indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span> 
  
```XML
<SendSMSAlertToRecipients>
   <Address/>
</SendSMSAlertToRecipients>
```

 <span data-ttu-id="d4839-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="d4839-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4839-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d4839-106">Attributes and elements</span></span>

<span data-ttu-id="d4839-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d4839-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4839-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d4839-108">Attributes</span></span>

<span data-ttu-id="d4839-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4839-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4839-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d4839-110">Child elements</span></span>

|<span data-ttu-id="d4839-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4839-111">**Element**</span></span>|<span data-ttu-id="d4839-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4839-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4839-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="d4839-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="d4839-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d4839-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4839-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d4839-115">Parent elements</span></span>

|<span data-ttu-id="d4839-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4839-116">**Element**</span></span>|<span data-ttu-id="d4839-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4839-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4839-118">Actions</span><span class="sxs-lookup"><span data-stu-id="d4839-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="d4839-119">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="d4839-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4839-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d4839-120">Text value</span></span>

<span data-ttu-id="d4839-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4839-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4839-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d4839-122">Remarks</span></span>

<span data-ttu-id="d4839-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4839-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4839-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d4839-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4839-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4839-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4839-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d4839-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d4839-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d4839-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4839-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d4839-128">Validation File</span></span>  <br/> |<span data-ttu-id="d4839-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4839-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4839-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d4839-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4839-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d4839-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4839-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d4839-132">See also</span></span>



- [<span data-ttu-id="d4839-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4839-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

