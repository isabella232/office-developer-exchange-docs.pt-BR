---
title: SendNotificationResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResult
api_type:
- schema
ms.assetid: fa9d6202-fa66-4f10-9858-53f4f1ce14bc
description: O elemento SendNotificationResult contém a resposta de um aplicativo cliente para uma notificação por push.
ms.openlocfilehash: 4ee9a0dda3d887f8fbfa2c2b34a9a077e7af37ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464886"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="5c403-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="5c403-103">SendNotificationResult</span></span>

<span data-ttu-id="5c403-104">O elemento **SendNotificationResult** contém a resposta de um aplicativo cliente para uma notificação por push.</span><span class="sxs-lookup"><span data-stu-id="5c403-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="5c403-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="5c403-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c403-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5c403-106">Attributes and elements</span></span>

<span data-ttu-id="5c403-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c403-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c403-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c403-108">Attributes</span></span>

<span data-ttu-id="5c403-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c403-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c403-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c403-110">Child elements</span></span>

|<span data-ttu-id="5c403-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c403-111">**Element**</span></span>|<span data-ttu-id="5c403-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c403-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c403-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="5c403-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="5c403-114">Descreve o status de uma assinatura push.</span><span class="sxs-lookup"><span data-stu-id="5c403-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c403-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c403-115">Parent elements</span></span>

<span data-ttu-id="5c403-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c403-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c403-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c403-117">Remarks</span></span>

<span data-ttu-id="5c403-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5c403-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c403-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5c403-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c403-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c403-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c403-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c403-121">Schema Name</span></span>  <br/> |<span data-ttu-id="5c403-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5c403-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c403-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c403-123">Validation File</span></span>  <br/> |<span data-ttu-id="5c403-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c403-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c403-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c403-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c403-126">False</span><span class="sxs-lookup"><span data-stu-id="5c403-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c403-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c403-127">See also</span></span>



- [<span data-ttu-id="5c403-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c403-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

