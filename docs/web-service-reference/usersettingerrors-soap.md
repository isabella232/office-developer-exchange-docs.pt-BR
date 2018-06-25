---
title: UserSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a9b94bae-cab9-412d-a811-801e849ed6c5
description: O elemento UserSettingErrors representa uma coleção de informações sobre as configurações que não puderam ser retornadas.
ms.openlocfilehash: 4477c30145d2cb187a4309d018512537af974ee8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838008"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="408df-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="408df-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="408df-104">O elemento **UserSettingErrors** representa uma coleção de informações sobre as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="408df-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="408df-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="408df-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="408df-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="408df-106">Attributes and elements</span></span>

<span data-ttu-id="408df-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="408df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="408df-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="408df-108">Attributes</span></span>

<span data-ttu-id="408df-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="408df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="408df-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="408df-110">Child elements</span></span>

|<span data-ttu-id="408df-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="408df-111">**Element**</span></span>|<span data-ttu-id="408df-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408df-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="408df-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="408df-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="408df-114">Representa um erro retornado ao recuperar uma configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="408df-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="408df-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="408df-115">Parent elements</span></span>

|<span data-ttu-id="408df-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="408df-116">**Element**</span></span>|<span data-ttu-id="408df-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408df-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="408df-118">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="408df-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="408df-119">Representa uma resposta a uma solicitação de GetUserSettings para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="408df-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="408df-120">Text value</span><span class="sxs-lookup"><span data-stu-id="408df-120">Text value</span></span>

<span data-ttu-id="408df-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="408df-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="408df-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="408df-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="408df-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="408df-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="408df-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="408df-124">Schema Name</span></span>  <br/> |<span data-ttu-id="408df-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="408df-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="408df-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="408df-126">Validation File</span></span>  <br/> |<span data-ttu-id="408df-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="408df-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="408df-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="408df-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="408df-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="408df-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="408df-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="408df-130">See also</span></span>



[<span data-ttu-id="408df-131">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="408df-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

