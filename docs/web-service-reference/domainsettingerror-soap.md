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
description: O elemento DomainSettingError representa um erro que ocorreu ao recuperar uma configuração de domínio. Isso representa um erro de uma solicitação GetDomainSettings.
ms.openlocfilehash: 189a614e7629033c8db2f60b8fd3679835a696ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530709"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="47411-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="47411-105">O elemento **DomainSettingError** representa um erro que ocorreu ao recuperar uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="47411-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="47411-106">Isso representa um erro de uma solicitação **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="47411-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="47411-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="47411-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47411-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="47411-108">Attributes and elements</span></span>

<span data-ttu-id="47411-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47411-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47411-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="47411-110">Attributes</span></span>

<span data-ttu-id="47411-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47411-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47411-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47411-112">Child elements</span></span>

|<span data-ttu-id="47411-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47411-113">**Element**</span></span>|<span data-ttu-id="47411-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47411-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47411-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="47411-116">Identifica o código de erro associado à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="47411-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="47411-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="47411-118">Contém a mensagem de erro associada à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="47411-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="47411-119">SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="47411-120">Representa o nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="47411-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47411-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47411-121">Parent elements</span></span>

|<span data-ttu-id="47411-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47411-122">**Element**</span></span>|<span data-ttu-id="47411-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47411-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47411-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="47411-125">Contém informações de erro sobre as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="47411-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47411-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="47411-126">Text value</span></span>

<span data-ttu-id="47411-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47411-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47411-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="47411-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47411-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="47411-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="47411-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47411-130">Schema Name</span></span>  <br/> |<span data-ttu-id="47411-131">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="47411-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="47411-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47411-132">Validation File</span></span>  <br/> |<span data-ttu-id="47411-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="47411-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47411-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47411-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="47411-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="47411-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47411-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="47411-136">See also</span></span>

- [<span data-ttu-id="47411-137">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="47411-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

