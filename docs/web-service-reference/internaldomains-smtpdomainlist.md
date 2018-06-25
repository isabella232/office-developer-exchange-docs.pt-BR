---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: O elemento InternalDomains identifica a lista de domínios de SMTP internos da organização.
ms.openlocfilehash: f37a31f4348a7eb0024656489f249dec349bc67b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823953"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="de3d4-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="de3d4-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="de3d4-104">O elemento **InternalDomains** identifica a lista de domínios de SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="de3d4-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="de3d4-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="de3d4-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de3d4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="de3d4-106">Attributes and elements</span></span>

<span data-ttu-id="de3d4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de3d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de3d4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="de3d4-108">Attributes</span></span>

<span data-ttu-id="de3d4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="de3d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de3d4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de3d4-110">Child elements</span></span>

|<span data-ttu-id="de3d4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de3d4-111">**Element**</span></span>|<span data-ttu-id="de3d4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de3d4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3d4-113">Domain</span><span class="sxs-lookup"><span data-stu-id="de3d4-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="de3d4-114">Identifica um único domínio SMTP.</span><span class="sxs-lookup"><span data-stu-id="de3d4-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de3d4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de3d4-115">Parent elements</span></span>

|<span data-ttu-id="de3d4-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de3d4-116">**Element**</span></span>|<span data-ttu-id="de3d4-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de3d4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3d4-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="de3d4-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="de3d4-119">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="de3d4-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="de3d4-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="de3d4-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="de3d4-121">Contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="de3d4-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de3d4-122">Text value</span><span class="sxs-lookup"><span data-stu-id="de3d4-122">Text value</span></span>

<span data-ttu-id="de3d4-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="de3d4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de3d4-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="de3d4-124">Remarks</span></span>

<span data-ttu-id="de3d4-125">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de3d4-125">This element is required.</span></span> 
  
<span data-ttu-id="de3d4-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="de3d4-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de3d4-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="de3d4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de3d4-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="de3d4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de3d4-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de3d4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="de3d4-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="de3d4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="de3d4-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de3d4-131">Validation File</span></span>  <br/> |<span data-ttu-id="de3d4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de3d4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de3d4-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de3d4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="de3d4-134">False</span><span class="sxs-lookup"><span data-stu-id="de3d4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de3d4-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="de3d4-135">See also</span></span>



- [<span data-ttu-id="de3d4-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de3d4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

