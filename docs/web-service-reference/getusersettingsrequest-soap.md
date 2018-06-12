---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: O elemento GetUserSettingsRequest representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.
ms.openlocfilehash: dc22570144a6947dc6e7042326c7416422680cc1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823702"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="90a2b-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="90a2b-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="90a2b-104">O elemento **GetUserSettingsRequest** representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="90a2b-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="90a2b-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="90a2b-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90a2b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="90a2b-106">Attributes and elements</span></span>

<span data-ttu-id="90a2b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90a2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90a2b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90a2b-108">Attributes</span></span>

<span data-ttu-id="90a2b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90a2b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90a2b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90a2b-110">Child elements</span></span>

|<span data-ttu-id="90a2b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90a2b-111">**Element**</span></span>|<span data-ttu-id="90a2b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90a2b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90a2b-113">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="90a2b-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="90a2b-114">Representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="90a2b-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="90a2b-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="90a2b-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="90a2b-116">Contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="90a2b-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="90a2b-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="90a2b-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="90a2b-118">Especifica a versão de servidor específico que o provedor gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="90a2b-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90a2b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90a2b-119">Parent elements</span></span>

<span data-ttu-id="90a2b-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90a2b-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="90a2b-121">Text value</span><span class="sxs-lookup"><span data-stu-id="90a2b-121">Text value</span></span>

<span data-ttu-id="90a2b-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90a2b-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90a2b-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="90a2b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90a2b-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="90a2b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="90a2b-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90a2b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="90a2b-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="90a2b-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="90a2b-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90a2b-127">Validation File</span></span>  <br/> |<span data-ttu-id="90a2b-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="90a2b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90a2b-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90a2b-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="90a2b-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="90a2b-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90a2b-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="90a2b-131">See also</span></span>



[<span data-ttu-id="90a2b-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="90a2b-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

