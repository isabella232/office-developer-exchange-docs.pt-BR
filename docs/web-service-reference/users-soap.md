---
title: Usuários (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: O elemento Users representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.
ms.openlocfilehash: 851447a2918e365b7c5d8812a61c9d425d26ffa2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461895"
---
# <a name="users-soap"></a><span data-ttu-id="21fd7-103">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="21fd7-103">Users (SOAP)</span></span>

<span data-ttu-id="21fd7-104">O elemento **Users** representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="21fd7-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="21fd7-105">**Usuários**</span><span class="sxs-lookup"><span data-stu-id="21fd7-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21fd7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="21fd7-106">Attributes and elements</span></span>

<span data-ttu-id="21fd7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="21fd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21fd7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="21fd7-108">Attributes</span></span>

<span data-ttu-id="21fd7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21fd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21fd7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="21fd7-110">Child elements</span></span>

|<span data-ttu-id="21fd7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="21fd7-111">**Element**</span></span>|<span data-ttu-id="21fd7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21fd7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21fd7-113">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="21fd7-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="21fd7-114">Representa o endereço de email de um usuário.</span><span class="sxs-lookup"><span data-stu-id="21fd7-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21fd7-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="21fd7-115">Parent elements</span></span>

|<span data-ttu-id="21fd7-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="21fd7-116">**Element**</span></span>|<span data-ttu-id="21fd7-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21fd7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21fd7-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="21fd7-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="21fd7-119">Representa uma solicitação para recuperar as configurações especificadas de um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="21fd7-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="21fd7-120">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="21fd7-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="21fd7-121">Contém as definições de configuração solicitadas e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="21fd7-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21fd7-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="21fd7-122">Text value</span></span>

<span data-ttu-id="21fd7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21fd7-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21fd7-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="21fd7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21fd7-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="21fd7-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="21fd7-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="21fd7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="21fd7-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="21fd7-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="21fd7-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="21fd7-128">Validation File</span></span>  <br/> |<span data-ttu-id="21fd7-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21fd7-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21fd7-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="21fd7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="21fd7-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="21fd7-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21fd7-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="21fd7-132">See also</span></span>



[<span data-ttu-id="21fd7-133">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="21fd7-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

