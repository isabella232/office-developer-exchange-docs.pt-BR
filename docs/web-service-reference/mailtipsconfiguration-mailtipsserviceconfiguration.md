---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: O elemento MailTipsConfiguration contém informações de configuração de serviço para o serviço de dicas de email.
ms.openlocfilehash: ea92af3ebb2d2f720e5823c5317d09d5bcdb3978
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824321"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="c5379-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="c5379-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="c5379-104">O elemento **MailTipsConfiguration** contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="c5379-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 <span data-ttu-id="c5379-105">**MailTipsServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c5379-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5379-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c5379-106">Attributes and elements</span></span>

<span data-ttu-id="c5379-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c5379-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5379-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c5379-108">Attributes</span></span>

<span data-ttu-id="c5379-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c5379-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5379-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c5379-110">Child elements</span></span>

|<span data-ttu-id="c5379-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c5379-111">**Element**</span></span>|<span data-ttu-id="c5379-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c5379-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5379-113">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="c5379-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="c5379-114">Indica se o serviço de dicas de email está disponível.</span><span class="sxs-lookup"><span data-stu-id="c5379-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="c5379-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5379-116">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="c5379-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="c5379-117">Indica o número máximo de destinatários que podem ser passados para a [operação GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c5379-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="c5379-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5379-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="c5379-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="c5379-120">Representa o tamanho de mensagem máximo que um destinatário pode aceitar.</span><span class="sxs-lookup"><span data-stu-id="c5379-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="c5379-121">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5379-122">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="c5379-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="c5379-123">Representa o limite de grande público para um cliente.</span><span class="sxs-lookup"><span data-stu-id="c5379-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="c5379-124">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5379-125">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="c5379-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="c5379-126">Indica se os consumidores da [operação GetMailTips](getmailtips-operation.md) têm que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.</span><span class="sxs-lookup"><span data-stu-id="c5379-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="c5379-127">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5379-128">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="c5379-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="c5379-129">Identifica a lista de domínios de SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="c5379-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="c5379-130">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5379-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5379-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c5379-131">Parent elements</span></span>

|<span data-ttu-id="c5379-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c5379-132">**Element**</span></span>|<span data-ttu-id="c5379-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c5379-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5379-134">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="c5379-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="c5379-135">Contém as definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="c5379-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5379-136">Text value</span><span class="sxs-lookup"><span data-stu-id="c5379-136">Text value</span></span>

<span data-ttu-id="c5379-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c5379-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5379-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="c5379-138">Remarks</span></span>

<span data-ttu-id="c5379-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5379-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5379-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c5379-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5379-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5379-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c5379-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c5379-142">Schema Name</span></span>  <br/> |<span data-ttu-id="c5379-143">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c5379-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c5379-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c5379-144">Validation File</span></span>  <br/> |<span data-ttu-id="c5379-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c5379-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c5379-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c5379-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5379-147">False</span><span class="sxs-lookup"><span data-stu-id="c5379-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5379-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="c5379-148">See also</span></span>



- [<span data-ttu-id="c5379-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c5379-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

