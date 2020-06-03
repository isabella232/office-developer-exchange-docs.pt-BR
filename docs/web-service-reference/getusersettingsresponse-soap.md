---
title: GetUserSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: O elemento GetUserSettingsResponse representa uma resposta a uma solicitação de operação do GetUserSettings (SOAP).
ms.openlocfilehash: a41a195a003789ddaef81f844e47aad689df0937
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530145"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="c2c7b-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2c7b-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="c2c7b-104">O elemento **GetUserSettingsResponse** representa uma resposta a uma solicitação de [operação do GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="c2c7b-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="c2c7b-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="c2c7b-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2c7b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c2c7b-106">Attributes and elements</span></span>

<span data-ttu-id="c2c7b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2c7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2c7b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2c7b-108">Attributes</span></span>

<span data-ttu-id="c2c7b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2c7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2c7b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2c7b-110">Child elements</span></span>

|<span data-ttu-id="c2c7b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2c7b-111">**Element**</span></span>|<span data-ttu-id="c2c7b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2c7b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2c7b-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2c7b-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="c2c7b-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="c2c7b-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="c2c7b-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2c7b-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="c2c7b-116">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="c2c7b-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="c2c7b-117">Userresponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2c7b-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="c2c7b-118">Contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="c2c7b-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2c7b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2c7b-119">Parent elements</span></span>

<span data-ttu-id="c2c7b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2c7b-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c2c7b-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c2c7b-121">Text value</span></span>

<span data-ttu-id="c2c7b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2c7b-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2c7b-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c2c7b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2c7b-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2c7b-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c2c7b-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2c7b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c2c7b-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c2c7b-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c2c7b-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2c7b-127">Validation File</span></span>  <br/> |<span data-ttu-id="c2c7b-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2c7b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2c7b-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2c7b-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2c7b-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c2c7b-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2c7b-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="c2c7b-131">See also</span></span>



[<span data-ttu-id="c2c7b-132">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2c7b-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

