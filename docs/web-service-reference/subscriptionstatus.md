---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: O elemento SubscriptionStatus descreve o status de uma inscrição de envio.
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837667"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="6e5ec-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="6e5ec-103">SubscriptionStatus</span></span>

<span data-ttu-id="6e5ec-104">O elemento **SubscriptionStatus** descreve o status de uma inscrição de envio.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="6e5ec-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="6e5ec-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e5ec-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6e5ec-106">Attributes and elements</span></span>

<span data-ttu-id="6e5ec-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e5ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e5ec-108">Attributes</span></span>

<span data-ttu-id="6e5ec-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e5ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e5ec-110">Child elements</span></span>

<span data-ttu-id="6e5ec-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e5ec-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e5ec-112">Parent elements</span></span>

|<span data-ttu-id="6e5ec-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e5ec-113">**Element**</span></span>|<span data-ttu-id="6e5ec-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e5ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e5ec-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="6e5ec-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="6e5ec-116">Contém a resposta do aplicativo cliente ' para uma notificação de push.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e5ec-117">Text value</span><span class="sxs-lookup"><span data-stu-id="6e5ec-117">Text value</span></span>

<span data-ttu-id="6e5ec-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-118">A text value is required.</span></span> <span data-ttu-id="6e5ec-119">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6e5ec-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="6e5ec-120">OK</span><span class="sxs-lookup"><span data-stu-id="6e5ec-120">OK</span></span>
    
- <span data-ttu-id="6e5ec-121">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="6e5ec-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6e5ec-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="6e5ec-122">Remarks</span></span>

<span data-ttu-id="6e5ec-123">Esse elemento descreve o status da assinatura.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="6e5ec-124">O aplicativo de cliente de assinatura push envia o status de volta para o computador que está executando o Exchange 2007 que possui a função de servidor de acesso para cliente instalada após cada notificação de push.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="6e5ec-125">Se o valor de **SubscriptionStatus** é igual o **cancelamento da assinatura**, o servidor de acesso para cliente interromperá o envio de notificações e encerrar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="6e5ec-126">Se o valor de **SubscriptionStatus** for igual a **Okey**, o servidor de acesso para cliente continuará enviar notificações.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="6e5ec-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6e5ec-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e5ec-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6e5ec-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e5ec-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e5ec-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e5ec-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e5ec-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6e5ec-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6e5ec-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e5ec-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e5ec-132">Validation File</span></span>  <br/> |<span data-ttu-id="6e5ec-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e5ec-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e5ec-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6e5ec-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e5ec-135">False</span><span class="sxs-lookup"><span data-stu-id="6e5ec-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e5ec-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="6e5ec-136">See also</span></span>



- [<span data-ttu-id="6e5ec-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6e5ec-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

