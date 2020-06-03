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
description: O elemento GetUserSettingsRequest representa uma solicitação para recuperar as configurações especificadas de um ou mais usuários.
ms.openlocfilehash: 353facb5d0bbf922a23b33cbaf6f9d2e7d82bd6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530159"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="58312-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58312-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="58312-104">O elemento **GetUserSettingsRequest** representa uma solicitação para recuperar as configurações especificadas de um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="58312-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="58312-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="58312-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58312-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58312-106">Attributes and elements</span></span>

<span data-ttu-id="58312-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58312-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58312-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58312-108">Attributes</span></span>

<span data-ttu-id="58312-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58312-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58312-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58312-110">Child elements</span></span>

|<span data-ttu-id="58312-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58312-111">**Element**</span></span>|<span data-ttu-id="58312-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58312-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58312-113">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58312-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="58312-114">Representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="58312-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="58312-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58312-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="58312-116">Contém os nomes das definições de configuração solicitadas.</span><span class="sxs-lookup"><span data-stu-id="58312-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="58312-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58312-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="58312-118">Especifica a versão de servidor específica que o provedor gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="58312-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58312-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58312-119">Parent elements</span></span>

<span data-ttu-id="58312-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58312-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="58312-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="58312-121">Text value</span></span>

<span data-ttu-id="58312-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58312-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58312-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58312-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58312-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="58312-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="58312-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58312-125">Schema Name</span></span>  <br/> |<span data-ttu-id="58312-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="58312-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="58312-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58312-127">Validation File</span></span>  <br/> |<span data-ttu-id="58312-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="58312-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="58312-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="58312-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="58312-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="58312-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58312-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="58312-131">See also</span></span>



[<span data-ttu-id="58312-132">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58312-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

