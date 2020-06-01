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
description: O elemento InternalDomains identifica a lista de domínios SMTP internos da organização.
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459963"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="9fd51-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="9fd51-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="9fd51-104">O elemento **InternalDomains** identifica a lista de domínios SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="9fd51-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="9fd51-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="9fd51-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fd51-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9fd51-106">Attributes and elements</span></span>

<span data-ttu-id="9fd51-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9fd51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fd51-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9fd51-108">Attributes</span></span>

<span data-ttu-id="9fd51-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9fd51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fd51-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9fd51-110">Child elements</span></span>

|<span data-ttu-id="9fd51-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fd51-111">**Element**</span></span>|<span data-ttu-id="9fd51-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fd51-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd51-113">Domínio</span><span class="sxs-lookup"><span data-stu-id="9fd51-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="9fd51-114">Identifica um único domínio SMTP.</span><span class="sxs-lookup"><span data-stu-id="9fd51-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9fd51-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9fd51-115">Parent elements</span></span>

|<span data-ttu-id="9fd51-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9fd51-116">**Element**</span></span>|<span data-ttu-id="9fd51-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9fd51-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fd51-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="9fd51-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="9fd51-119">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="9fd51-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="9fd51-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fd51-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="9fd51-121">Contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="9fd51-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fd51-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9fd51-122">Text value</span></span>

<span data-ttu-id="9fd51-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9fd51-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9fd51-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="9fd51-124">Remarks</span></span>

<span data-ttu-id="9fd51-125">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fd51-125">This element is required.</span></span> 
  
<span data-ttu-id="9fd51-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fd51-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fd51-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9fd51-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fd51-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="9fd51-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fd51-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9fd51-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9fd51-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9fd51-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fd51-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9fd51-131">Validation File</span></span>  <br/> |<span data-ttu-id="9fd51-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9fd51-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fd51-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9fd51-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9fd51-134">False</span><span class="sxs-lookup"><span data-stu-id="9fd51-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9fd51-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fd51-135">See also</span></span>



- [<span data-ttu-id="9fd51-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fd51-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

