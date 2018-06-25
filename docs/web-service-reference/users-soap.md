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
description: O elemento de usuários representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.
ms.openlocfilehash: d7655f0020a315dcb32adbbc58610ca0e630c1fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838000"
---
# <a name="users-soap"></a><span data-ttu-id="8c7be-103">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8c7be-103">Users (SOAP)</span></span>

<span data-ttu-id="8c7be-104">O elemento de **usuários** representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="8c7be-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="8c7be-105">**Usuários**</span><span class="sxs-lookup"><span data-stu-id="8c7be-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c7be-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8c7be-106">Attributes and elements</span></span>

<span data-ttu-id="8c7be-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8c7be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c7be-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8c7be-108">Attributes</span></span>

<span data-ttu-id="8c7be-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c7be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c7be-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8c7be-110">Child elements</span></span>

|<span data-ttu-id="8c7be-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8c7be-111">**Element**</span></span>|<span data-ttu-id="8c7be-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c7be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c7be-113">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8c7be-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="8c7be-114">Representa o endereço de email de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8c7be-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c7be-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8c7be-115">Parent elements</span></span>

|<span data-ttu-id="8c7be-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8c7be-116">**Element**</span></span>|<span data-ttu-id="8c7be-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c7be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c7be-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8c7be-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="8c7be-119">Representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="8c7be-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="8c7be-120">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8c7be-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="8c7be-121">Contém as definições de configuração solicitado e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="8c7be-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c7be-122">Text value</span><span class="sxs-lookup"><span data-stu-id="8c7be-122">Text value</span></span>

<span data-ttu-id="8c7be-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c7be-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c7be-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8c7be-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c7be-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="8c7be-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8c7be-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8c7be-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8c7be-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="8c7be-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8c7be-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8c7be-128">Validation File</span></span>  <br/> |<span data-ttu-id="8c7be-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8c7be-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8c7be-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8c7be-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8c7be-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="8c7be-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c7be-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="8c7be-132">See also</span></span>



[<span data-ttu-id="8c7be-133">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8c7be-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

