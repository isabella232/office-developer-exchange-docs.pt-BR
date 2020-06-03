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
description: O elemento SubscriptionStatus descreve o status de uma assinatura push.
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530941"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="98f66-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="98f66-103">SubscriptionStatus</span></span>

<span data-ttu-id="98f66-104">O elemento **SubscriptionStatus** descreve o status de uma assinatura push.</span><span class="sxs-lookup"><span data-stu-id="98f66-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="98f66-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="98f66-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98f66-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="98f66-106">Attributes and elements</span></span>

<span data-ttu-id="98f66-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="98f66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98f66-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="98f66-108">Attributes</span></span>

<span data-ttu-id="98f66-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98f66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98f66-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="98f66-110">Child elements</span></span>

<span data-ttu-id="98f66-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98f66-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98f66-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="98f66-112">Parent elements</span></span>

|<span data-ttu-id="98f66-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="98f66-113">**Element**</span></span>|<span data-ttu-id="98f66-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98f66-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98f66-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="98f66-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="98f66-116">Contém a resposta do aplicativo cliente ' para uma notificação por push.</span><span class="sxs-lookup"><span data-stu-id="98f66-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98f66-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="98f66-117">Text value</span></span>

<span data-ttu-id="98f66-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98f66-118">A text value is required.</span></span> <span data-ttu-id="98f66-119">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="98f66-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="98f66-120">OK</span><span class="sxs-lookup"><span data-stu-id="98f66-120">OK</span></span>
    
- <span data-ttu-id="98f66-121">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="98f66-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="98f66-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="98f66-122">Remarks</span></span>

<span data-ttu-id="98f66-123">Este elemento descreve o status da assinatura.</span><span class="sxs-lookup"><span data-stu-id="98f66-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="98f66-124">O aplicativo cliente de assinatura push envia o status de volta para o computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada após cada notificação por push.</span><span class="sxs-lookup"><span data-stu-id="98f66-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="98f66-125">Se o valor **SubscriptionStatus** for igual a **unsubscribe**, o servidor de acesso para cliente interromperá o envio de notificações e encerrará a assinatura.</span><span class="sxs-lookup"><span data-stu-id="98f66-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="98f66-126">Se o valor **SubscriptionStatus** for igual a **OK**, o servidor de acesso para cliente continuará a enviar notificações.</span><span class="sxs-lookup"><span data-stu-id="98f66-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="98f66-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="98f66-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98f66-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="98f66-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98f66-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="98f66-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98f66-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="98f66-130">Schema Name</span></span>  <br/> |<span data-ttu-id="98f66-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="98f66-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98f66-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="98f66-132">Validation File</span></span>  <br/> |<span data-ttu-id="98f66-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98f66-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98f66-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="98f66-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="98f66-135">False</span><span class="sxs-lookup"><span data-stu-id="98f66-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98f66-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="98f66-136">See also</span></span>



- [<span data-ttu-id="98f66-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="98f66-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

