---
title: PlayOnPhoneGreeting (serviço Web da UM)
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
description: O elemento PlayOnPhoneGreeting define uma solicitação para reproduzir uma saudação de Unificação de mensagens em um telefone.
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529921"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="3c478-103">PlayOnPhoneGreeting (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="3c478-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="3c478-104">O elemento **PlayOnPhoneGreeting** define uma solicitação para reproduzir uma saudação de Unificação de mensagens em um telefone.</span><span class="sxs-lookup"><span data-stu-id="3c478-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="3c478-105">PlayOnPhoneGreeting (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="3c478-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="3c478-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="3c478-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c478-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3c478-107">Attributes and elements</span></span>

<span data-ttu-id="3c478-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c478-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c478-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c478-109">Attributes</span></span>

<span data-ttu-id="3c478-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c478-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c478-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c478-111">Child elements</span></span>

|<span data-ttu-id="3c478-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3c478-112">**Element**</span></span>|<span data-ttu-id="3c478-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3c478-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c478-114">Greetingtype (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="3c478-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="3c478-115">Define o tipo de saudação a ser usado em uma solicitação de [operação do PlayOnPhoneGreeting (serviço Web da um)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="3c478-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="3c478-116">dialstring (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="3c478-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="3c478-117">Contém o valor do número de telefone a ser discado.</span><span class="sxs-lookup"><span data-stu-id="3c478-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c478-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c478-118">Parent elements</span></span>

<span data-ttu-id="3c478-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c478-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3c478-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3c478-120">Text value</span></span>

<span data-ttu-id="3c478-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c478-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c478-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3c478-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c478-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c478-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c478-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c478-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3c478-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="3c478-125">Messages</span></span>  <br/> |
|<span data-ttu-id="3c478-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c478-126">Validation File</span></span>  <br/> |<span data-ttu-id="3c478-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3c478-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c478-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3c478-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c478-129">False</span><span class="sxs-lookup"><span data-stu-id="3c478-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c478-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="3c478-130">See also</span></span>



[<span data-ttu-id="3c478-131">Operação PlayOnPhoneGreeting (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="3c478-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

