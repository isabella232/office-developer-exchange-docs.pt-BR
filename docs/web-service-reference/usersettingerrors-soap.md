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
ms.openlocfilehash: a6cc0fe114bd511dc4136532986b552c28b0d5c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467120"
---
# <a name="usersettingerrors-soap"></a><span data-ttu-id="e1ebe-103">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e1ebe-103">UserSettingErrors (SOAP)</span></span>

<span data-ttu-id="e1ebe-104">O elemento **UserSettingErrors** representa uma coleção de informações sobre as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="e1ebe-104">The **UserSettingErrors** element represents a collection of information about settings that could not be returned.</span></span> 
  
```XML
<UserSettingErrors>
    <UserSettingError/>
</UserSettingErrors>
```

 <span data-ttu-id="e1ebe-105">**UserSettingErrors**</span><span class="sxs-lookup"><span data-stu-id="e1ebe-105">**UserSettingErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1ebe-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1ebe-106">Attributes and elements</span></span>

<span data-ttu-id="e1ebe-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1ebe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1ebe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1ebe-108">Attributes</span></span>

<span data-ttu-id="e1ebe-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1ebe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1ebe-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1ebe-110">Child elements</span></span>

|<span data-ttu-id="e1ebe-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1ebe-111">**Element**</span></span>|<span data-ttu-id="e1ebe-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1ebe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1ebe-113">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e1ebe-113">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="e1ebe-114">Representa um erro retornado ao recuperar uma configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1ebe-114">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1ebe-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1ebe-115">Parent elements</span></span>

|<span data-ttu-id="e1ebe-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1ebe-116">**Element**</span></span>|<span data-ttu-id="e1ebe-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1ebe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1ebe-118">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e1ebe-118">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="e1ebe-119">Representa uma resposta a uma solicitação GetUserSettings para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="e1ebe-119">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1ebe-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e1ebe-120">Text value</span></span>

<span data-ttu-id="e1ebe-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1ebe-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1ebe-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e1ebe-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1ebe-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1ebe-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e1ebe-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1ebe-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e1ebe-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="e1ebe-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e1ebe-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1ebe-126">Validation File</span></span>  <br/> |<span data-ttu-id="e1ebe-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e1ebe-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1ebe-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e1ebe-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1ebe-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="e1ebe-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1ebe-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1ebe-130">See also</span></span>



[<span data-ttu-id="e1ebe-131">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e1ebe-131">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

