---
title: SetPlayOnPhoneDialString (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: O elemento SetPlayOnPhoneDialString define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações PlayOnPhone (serviço Web da UM) e PlayOnPhoneGreeting (serviço Web da UM).
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458625"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="21ab6-103">SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="21ab6-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="21ab6-104">O elemento **SetPlayOnPhoneDialString** define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações [PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e [PLAYONPHONEGREETING (serviço Web da um)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="21ab6-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="21ab6-105">SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="21ab6-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="21ab6-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="21ab6-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21ab6-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="21ab6-107">Attributes and elements</span></span>

<span data-ttu-id="21ab6-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="21ab6-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21ab6-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="21ab6-109">Attributes</span></span>

<span data-ttu-id="21ab6-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21ab6-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21ab6-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="21ab6-111">Child elements</span></span>

|<span data-ttu-id="21ab6-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="21ab6-112">**Element**</span></span>|<span data-ttu-id="21ab6-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21ab6-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21ab6-114">dialstring (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="21ab6-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="21ab6-115">O número de telefone a ser definido como a cadeia de caracteres de discagem padrão.</span><span class="sxs-lookup"><span data-stu-id="21ab6-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21ab6-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="21ab6-116">Parent elements</span></span>

<span data-ttu-id="21ab6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21ab6-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="21ab6-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="21ab6-118">Text value</span></span>

<span data-ttu-id="21ab6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21ab6-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21ab6-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="21ab6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21ab6-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="21ab6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21ab6-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="21ab6-122">Schema Name</span></span>  <br/> |<span data-ttu-id="21ab6-123">Mensagens</span><span class="sxs-lookup"><span data-stu-id="21ab6-123">Messages</span></span>  <br/> |
|<span data-ttu-id="21ab6-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="21ab6-124">Validation File</span></span>  <br/> |<span data-ttu-id="21ab6-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21ab6-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21ab6-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="21ab6-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="21ab6-127">False</span><span class="sxs-lookup"><span data-stu-id="21ab6-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21ab6-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="21ab6-128">See also</span></span>



[<span data-ttu-id="21ab6-129">Operação SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="21ab6-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

