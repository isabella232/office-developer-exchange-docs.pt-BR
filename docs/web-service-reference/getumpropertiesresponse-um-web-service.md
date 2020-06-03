---
title: GetUMPropertiesResponse (serviço Web da UM)
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
description: O elemento GetUMPropertiesResponse define uma resposta a uma solicitação de operação GetUMProperties (serviço Web da UM).
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459122"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="d7b2e-103">GetUMPropertiesResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="d7b2e-104">O elemento **GetUMPropertiesResponse** define uma resposta a uma solicitação de [operação GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d7b2e-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="d7b2e-105">GetUMPropertiesResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="d7b2e-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="d7b2e-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7b2e-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d7b2e-107">Attributes and elements</span></span>

<span data-ttu-id="d7b2e-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7b2e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7b2e-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7b2e-109">Attributes</span></span>

<span data-ttu-id="d7b2e-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7b2e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7b2e-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7b2e-111">Child elements</span></span>

|<span data-ttu-id="d7b2e-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7b2e-112">**Element**</span></span>|<span data-ttu-id="d7b2e-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7b2e-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7b2e-114">MissedCallNotificationEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="d7b2e-115">Indica se as notificações de chamadas perdidas estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="d7b2e-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="d7b2e-116">PlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="d7b2e-117">Contém a cadeia de caracteres de discagem padrão a ser usada para a [operação PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço da um)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="d7b2e-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="d7b2e-118">TelephoneAccessNumbers (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="d7b2e-119">Contém a lista de números de telefone que o usuário pode usar para acessar a Unificação de mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="d7b2e-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="d7b2e-120">TelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="d7b2e-121">Contém o identificador da pasta de email a partir da qual a Unificação de mensagens lerá as mensagens por telefone.</span><span class="sxs-lookup"><span data-stu-id="d7b2e-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7b2e-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7b2e-122">Parent elements</span></span>

<span data-ttu-id="d7b2e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7b2e-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d7b2e-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d7b2e-124">Text value</span></span>

<span data-ttu-id="d7b2e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7b2e-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7b2e-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d7b2e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7b2e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7b2e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7b2e-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7b2e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d7b2e-129">Mensagens</span><span class="sxs-lookup"><span data-stu-id="d7b2e-129">Messages</span></span>  <br/> |
|<span data-ttu-id="d7b2e-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7b2e-130">Validation File</span></span>  <br/> |<span data-ttu-id="d7b2e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7b2e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7b2e-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d7b2e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7b2e-133">False</span><span class="sxs-lookup"><span data-stu-id="d7b2e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7b2e-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7b2e-134">See also</span></span>



[<span data-ttu-id="d7b2e-135">Operação GetUMProperties (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7b2e-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

