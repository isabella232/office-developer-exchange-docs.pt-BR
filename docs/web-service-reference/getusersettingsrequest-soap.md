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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823702"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="0b947-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b947-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="0b947-104">O elemento **GetUserSettingsRequest** representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="0b947-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="0b947-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="0b947-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b947-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0b947-106">Attributes and elements</span></span>

<span data-ttu-id="0b947-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b947-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b947-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b947-108">Attributes</span></span>

<span data-ttu-id="0b947-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b947-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b947-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b947-110">Child elements</span></span>

|<span data-ttu-id="0b947-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b947-111">**Element**</span></span>|<span data-ttu-id="0b947-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b947-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b947-113">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b947-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="0b947-114">Representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="0b947-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="0b947-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b947-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="0b947-116">Contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="0b947-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="0b947-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b947-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="0b947-118">Especifica a versão de servidor específico que o provedor gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="0b947-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b947-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b947-119">Parent elements</span></span>

<span data-ttu-id="0b947-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b947-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0b947-121">Text value</span><span class="sxs-lookup"><span data-stu-id="0b947-121">Text value</span></span>

<span data-ttu-id="0b947-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b947-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b947-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0b947-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b947-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b947-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0b947-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b947-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0b947-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0b947-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0b947-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b947-127">Validation File</span></span>  <br/> |<span data-ttu-id="0b947-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b947-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b947-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0b947-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b947-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0b947-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b947-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="0b947-131">See also</span></span>



[<span data-ttu-id="0b947-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0b947-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

