---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: O elemento RedirectTarget (SOAP) contém o destino da URL de redirecionamento ou endereço de email.
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462196"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="c9c05-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9c05-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="c9c05-104">O elemento [RedirectTarget (SOAP)](redirecttarget-soap.md) contém o destino da URL de redirecionamento ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="c9c05-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="c9c05-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c9c05-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9c05-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c9c05-106">Attributes and elements</span></span>

<span data-ttu-id="c9c05-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9c05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9c05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9c05-108">Attributes</span></span>

<span data-ttu-id="c9c05-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9c05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9c05-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9c05-110">Child elements</span></span>

<span data-ttu-id="c9c05-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9c05-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9c05-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9c05-112">Parent elements</span></span>

|<span data-ttu-id="c9c05-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9c05-113">**Element**</span></span>|<span data-ttu-id="c9c05-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9c05-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9c05-115">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9c05-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="c9c05-116">Representa uma resposta a uma solicitação GetUserSettings para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="c9c05-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="c9c05-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9c05-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="c9c05-118">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="c9c05-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9c05-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c9c05-119">Text value</span></span>

<span data-ttu-id="c9c05-120">O valor de texto contém o destino da URL de redirecionamento ou o endereço de email que deve ser usado para uma solicitação subsequente de GetUserSettings ou GetDomainSettings.</span><span class="sxs-lookup"><span data-stu-id="c9c05-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9c05-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c9c05-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9c05-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9c05-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c9c05-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9c05-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c9c05-124">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c9c05-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c9c05-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9c05-125">Validation File</span></span>  <br/> |<span data-ttu-id="c9c05-126">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c9c05-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9c05-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c9c05-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9c05-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c9c05-128">True</span></span>  <br/> |
   

