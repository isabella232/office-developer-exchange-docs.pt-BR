---
title: PlayOnPhoneGreeting (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: O elemento de PlayOnPhoneGreeting define uma solicitação para reproduzir um Unificação de mensagens em um telefone de saudação.
ms.openlocfilehash: c30140fc60b9e902517b4cc18deb9b61efa61e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824836"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="5cd27-103">PlayOnPhoneGreeting (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5cd27-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="5cd27-104">O elemento de **PlayOnPhoneGreeting** define uma solicitação para reproduzir um Unificação de mensagens em um telefone de saudação.</span><span class="sxs-lookup"><span data-stu-id="5cd27-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="5cd27-105">PlayOnPhoneGreeting (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5cd27-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="5cd27-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="5cd27-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cd27-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5cd27-107">Attributes and elements</span></span>

<span data-ttu-id="5cd27-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5cd27-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cd27-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="5cd27-109">Attributes</span></span>

<span data-ttu-id="5cd27-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5cd27-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cd27-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5cd27-111">Child elements</span></span>

|<span data-ttu-id="5cd27-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5cd27-112">**Element**</span></span>|<span data-ttu-id="5cd27-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5cd27-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cd27-114">GreetingType (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5cd27-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="5cd27-115">Define o tipo de saudação a ser usado em uma solicitação de [operação PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="5cd27-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="5cd27-116">dialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5cd27-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="5cd27-117">Contém o valor para o número de telefone discar.</span><span class="sxs-lookup"><span data-stu-id="5cd27-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cd27-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5cd27-118">Parent elements</span></span>

<span data-ttu-id="5cd27-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5cd27-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5cd27-120">Text value</span><span class="sxs-lookup"><span data-stu-id="5cd27-120">Text value</span></span>

<span data-ttu-id="5cd27-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5cd27-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cd27-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5cd27-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cd27-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5cd27-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5cd27-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5cd27-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5cd27-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="5cd27-125">Messages</span></span>  <br/> |
|<span data-ttu-id="5cd27-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5cd27-126">Validation File</span></span>  <br/> |<span data-ttu-id="5cd27-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5cd27-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5cd27-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5cd27-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cd27-129">False</span><span class="sxs-lookup"><span data-stu-id="5cd27-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cd27-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="5cd27-130">See also</span></span>



[<span data-ttu-id="5cd27-131">Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5cd27-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

