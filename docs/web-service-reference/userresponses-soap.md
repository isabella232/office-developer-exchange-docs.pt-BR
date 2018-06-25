---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: O elemento UserResponses contém as definições de configuração para cada usuário solicitado.
ms.openlocfilehash: bee7f3c9a95c1facfe0adc990516dfa323d9c8cf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837995"
---
# <a name="userresponses-soap"></a><span data-ttu-id="895a1-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="895a1-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="895a1-104">O elemento **UserResponses** contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="895a1-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="895a1-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="895a1-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="895a1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="895a1-106">Attributes and elements</span></span>

<span data-ttu-id="895a1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="895a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="895a1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="895a1-108">Attributes</span></span>

<span data-ttu-id="895a1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="895a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="895a1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="895a1-110">Child elements</span></span>

|<span data-ttu-id="895a1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="895a1-111">**Element**</span></span>|<span data-ttu-id="895a1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="895a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="895a1-113">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="895a1-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="895a1-114">Representa uma resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="895a1-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="895a1-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="895a1-115">Parent elements</span></span>

|<span data-ttu-id="895a1-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="895a1-116">**Element**</span></span>|<span data-ttu-id="895a1-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="895a1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="895a1-118">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="895a1-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="895a1-119">Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="895a1-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="895a1-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="895a1-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="895a1-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="895a1-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="895a1-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="895a1-122">Schema Name</span></span>  <br/> |<span data-ttu-id="895a1-123">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="895a1-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="895a1-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="895a1-124">Validation File</span></span>  <br/> |<span data-ttu-id="895a1-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="895a1-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="895a1-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="895a1-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="895a1-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="895a1-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="895a1-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="895a1-128">See also</span></span>



[<span data-ttu-id="895a1-129">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="895a1-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

