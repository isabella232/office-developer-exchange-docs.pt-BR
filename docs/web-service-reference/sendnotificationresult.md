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
description: O elemento SendNotificationResult contém a resposta de um aplicativo cliente para uma notificação de push.
ms.openlocfilehash: 9acaa396430cf4e06a9c996834874d19dcab50ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825350"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="780a9-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="780a9-103">SendNotificationResult</span></span>

<span data-ttu-id="780a9-104">O elemento **SendNotificationResult** contém a resposta de um aplicativo cliente para uma notificação de push.</span><span class="sxs-lookup"><span data-stu-id="780a9-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="780a9-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="780a9-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="780a9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="780a9-106">Attributes and elements</span></span>

<span data-ttu-id="780a9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="780a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="780a9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="780a9-108">Attributes</span></span>

<span data-ttu-id="780a9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="780a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="780a9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="780a9-110">Child elements</span></span>

|<span data-ttu-id="780a9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="780a9-111">**Element**</span></span>|<span data-ttu-id="780a9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="780a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="780a9-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="780a9-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="780a9-114">Descreve o status de uma inscrição de envio.</span><span class="sxs-lookup"><span data-stu-id="780a9-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="780a9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="780a9-115">Parent elements</span></span>

<span data-ttu-id="780a9-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="780a9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="780a9-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="780a9-117">Remarks</span></span>

<span data-ttu-id="780a9-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="780a9-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="780a9-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="780a9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="780a9-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="780a9-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="780a9-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="780a9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="780a9-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="780a9-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="780a9-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="780a9-123">Validation File</span></span>  <br/> |<span data-ttu-id="780a9-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="780a9-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="780a9-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="780a9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="780a9-126">False</span><span class="sxs-lookup"><span data-stu-id="780a9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="780a9-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="780a9-127">See also</span></span>



- [<span data-ttu-id="780a9-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="780a9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

