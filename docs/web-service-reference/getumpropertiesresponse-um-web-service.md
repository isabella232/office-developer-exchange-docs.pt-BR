---
title: GetUMPropertiesResponse (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: O elemento de GetUMPropertiesResponse define uma resposta a uma solicitação do GetUMProperties operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823685"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="d0494-103">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="d0494-104">O elemento de **GetUMPropertiesResponse** define uma resposta a uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d0494-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="d0494-105">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="d0494-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="d0494-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0494-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d0494-107">Attributes and elements</span></span>

<span data-ttu-id="d0494-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d0494-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0494-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="d0494-109">Attributes</span></span>

<span data-ttu-id="d0494-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0494-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0494-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d0494-111">Child elements</span></span>

|<span data-ttu-id="d0494-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d0494-112">**Element**</span></span>|<span data-ttu-id="d0494-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0494-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0494-114">MissedCallNotificationEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="d0494-115">Indica se as notificações de chamadas perdidas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="d0494-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="d0494-116">PlayOnPhoneDialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="d0494-117">Contém a cadeia de caracteres de discagem padrão a ser usado para a [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) e a [operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="d0494-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="d0494-118">TelephoneAccessNumbers (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="d0494-119">Contém a lista de números de telefone que o usuário pode usar para acessar a Unificação de mensagens por meio de um telefone.</span><span class="sxs-lookup"><span data-stu-id="d0494-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="d0494-120">TelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="d0494-121">Contém o identificador para a pasta de email do qual Unificação de mensagens lê as mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="d0494-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0494-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d0494-122">Parent elements</span></span>

<span data-ttu-id="d0494-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0494-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d0494-124">Text value</span><span class="sxs-lookup"><span data-stu-id="d0494-124">Text value</span></span>

<span data-ttu-id="d0494-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d0494-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0494-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d0494-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0494-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="d0494-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0494-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d0494-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d0494-129">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d0494-129">Messages</span></span>  <br/> |
|<span data-ttu-id="d0494-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d0494-130">Validation File</span></span>  <br/> |<span data-ttu-id="d0494-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0494-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0494-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d0494-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0494-133">False</span><span class="sxs-lookup"><span data-stu-id="d0494-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0494-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="d0494-134">See also</span></span>



[<span data-ttu-id="d0494-135">Operação de GetUMProperties (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="d0494-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

