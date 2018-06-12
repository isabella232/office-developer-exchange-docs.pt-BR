---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: O elemento DomainSettingError representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma solicitação de GetDomainSettings.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751926"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="13149-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="13149-105">O elemento **DomainSettingError** representa um erro que ocorreu durante a recuperação de uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="13149-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="13149-106">Isso representa um erro de uma solicitação de **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="13149-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="13149-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="13149-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13149-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="13149-108">Attributes and elements</span></span>

<span data-ttu-id="13149-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="13149-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13149-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="13149-110">Attributes</span></span>

<span data-ttu-id="13149-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="13149-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13149-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="13149-112">Child elements</span></span>

|<span data-ttu-id="13149-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13149-113">**Element**</span></span>|<span data-ttu-id="13149-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13149-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13149-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="13149-116">Identifica o código de erro que está associado à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="13149-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="13149-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="13149-118">Contém a mensagem de erro que está associada à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="13149-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="13149-119">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="13149-120">Representa o nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="13149-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13149-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="13149-121">Parent elements</span></span>

|<span data-ttu-id="13149-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13149-122">**Element**</span></span>|<span data-ttu-id="13149-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13149-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13149-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="13149-125">Contém informações de erro para as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="13149-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13149-126">Text value</span><span class="sxs-lookup"><span data-stu-id="13149-126">Text value</span></span>

<span data-ttu-id="13149-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="13149-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13149-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="13149-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13149-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="13149-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="13149-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="13149-130">Schema Name</span></span>  <br/> |<span data-ttu-id="13149-131">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="13149-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="13149-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="13149-132">Validation File</span></span>  <br/> |<span data-ttu-id="13149-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="13149-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="13149-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="13149-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="13149-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="13149-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13149-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="13149-136">See also</span></span>

- [<span data-ttu-id="13149-137">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="13149-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

