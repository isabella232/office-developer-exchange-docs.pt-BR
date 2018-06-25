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
description: O elemento RedirectTarget (SOAP) contém o destino do endereço de email ou a URL de redirecionamento.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825019"
---
# <a name="redirecttarget-soap"></a><span data-ttu-id="14aa9-103">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14aa9-103">RedirectTarget (SOAP)</span></span>

<span data-ttu-id="14aa9-104">O elemento [RedirectTarget (SOAP)](redirecttarget-soap.md) contém o destino do endereço de email ou a URL de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="14aa9-104">The [RedirectTarget (SOAP)](redirecttarget-soap.md) element contains the target of the redirection URL or e-mail address.</span></span> 
  
```XML
<RedirectTarget/>
```

 <span data-ttu-id="14aa9-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="14aa9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14aa9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="14aa9-106">Attributes and elements</span></span>

<span data-ttu-id="14aa9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="14aa9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14aa9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="14aa9-108">Attributes</span></span>

<span data-ttu-id="14aa9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14aa9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14aa9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="14aa9-110">Child elements</span></span>

<span data-ttu-id="14aa9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14aa9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14aa9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="14aa9-112">Parent elements</span></span>

|<span data-ttu-id="14aa9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14aa9-113">**Element**</span></span>|<span data-ttu-id="14aa9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14aa9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14aa9-115">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="14aa9-115">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="14aa9-116">Representa uma resposta a uma solicitação de GetUserSettings para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="14aa9-116">Represents a response to a GetUserSettings request for an individual user.</span></span>  <br/> |
|[<span data-ttu-id="14aa9-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14aa9-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="14aa9-118">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="14aa9-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14aa9-119">Text value</span><span class="sxs-lookup"><span data-stu-id="14aa9-119">Text value</span></span>

<span data-ttu-id="14aa9-120">O valor de texto contém o destino do redirecionamento URL ou endereço de email que deve ser usado para um GetUserSettings subsequentes ou GetDomainSettings solicitação.</span><span class="sxs-lookup"><span data-stu-id="14aa9-120">The text value contains the target of the redirection URL or e-mail address that should be used for a subsequent GetUserSettings or GetDomainSettings request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14aa9-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="14aa9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14aa9-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="14aa9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="14aa9-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="14aa9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="14aa9-124">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="14aa9-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="14aa9-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="14aa9-125">Validation File</span></span>  <br/> |<span data-ttu-id="14aa9-126">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="14aa9-126">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14aa9-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="14aa9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="14aa9-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="14aa9-128">True</span></span>  <br/> |
   

