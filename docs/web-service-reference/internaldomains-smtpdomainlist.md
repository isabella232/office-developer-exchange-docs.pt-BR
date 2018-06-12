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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823953"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="bcc56-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="bcc56-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="bcc56-104">O elemento **InternalDomains** identifica a lista de domínios de SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="bcc56-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="bcc56-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="bcc56-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcc56-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bcc56-106">Attributes and elements</span></span>

<span data-ttu-id="bcc56-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bcc56-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcc56-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bcc56-108">Attributes</span></span>

<span data-ttu-id="bcc56-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bcc56-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcc56-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bcc56-110">Child elements</span></span>

|<span data-ttu-id="bcc56-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bcc56-111">**Element**</span></span>|<span data-ttu-id="bcc56-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bcc56-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcc56-113">Domain</span><span class="sxs-lookup"><span data-stu-id="bcc56-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="bcc56-114">Identifica um único domínio SMTP.</span><span class="sxs-lookup"><span data-stu-id="bcc56-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcc56-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bcc56-115">Parent elements</span></span>

|<span data-ttu-id="bcc56-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bcc56-116">**Element**</span></span>|<span data-ttu-id="bcc56-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bcc56-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcc56-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="bcc56-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="bcc56-119">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="bcc56-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="bcc56-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="bcc56-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="bcc56-121">Contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="bcc56-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bcc56-122">Text value</span><span class="sxs-lookup"><span data-stu-id="bcc56-122">Text value</span></span>

<span data-ttu-id="bcc56-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bcc56-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bcc56-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="bcc56-124">Remarks</span></span>

<span data-ttu-id="bcc56-125">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcc56-125">This element is required.</span></span> 
  
<span data-ttu-id="bcc56-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcc56-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcc56-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bcc56-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcc56-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="bcc56-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bcc56-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bcc56-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bcc56-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bcc56-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bcc56-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bcc56-131">Validation File</span></span>  <br/> |<span data-ttu-id="bcc56-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bcc56-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bcc56-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bcc56-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcc56-134">False</span><span class="sxs-lookup"><span data-stu-id="bcc56-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcc56-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="bcc56-135">See also</span></span>



- [<span data-ttu-id="bcc56-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bcc56-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

