---
title: Agindo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: O elemento agindo identifica quem o chamador está enviando como.
ms.openlocfilehash: 175a03018ee3529ec595dbe9afb7dc61ad6afc35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529697"
---
# <a name="actingas"></a><span data-ttu-id="cb6fe-103">Agindo</span><span class="sxs-lookup"><span data-stu-id="cb6fe-103">ActingAs</span></span>

<span data-ttu-id="cb6fe-104">O elemento **agindo** identifica quem o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="cb6fe-105">**EmailAddresstype**</span><span class="sxs-lookup"><span data-stu-id="cb6fe-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb6fe-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cb6fe-106">Attributes and elements</span></span>

<span data-ttu-id="cb6fe-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb6fe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cb6fe-108">Attributes</span></span>

<span data-ttu-id="cb6fe-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb6fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb6fe-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cb6fe-110">Child elements</span></span>

|<span data-ttu-id="cb6fe-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb6fe-111">**Element**</span></span>|<span data-ttu-id="cb6fe-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb6fe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb6fe-113">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="cb6fe-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="cb6fe-114">Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="cb6fe-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cb6fe-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="cb6fe-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="cb6fe-117">Define o roteamento usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="cb6fe-118">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-118">The default is SMTP.</span></span> <span data-ttu-id="cb6fe-119">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb6fe-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cb6fe-120">Parent elements</span></span>

|<span data-ttu-id="cb6fe-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb6fe-121">**Element**</span></span>|<span data-ttu-id="cb6fe-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb6fe-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb6fe-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb6fe-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="cb6fe-124">Define uma solicitação **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="cb6fe-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb6fe-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb6fe-125">Remarks</span></span>

<span data-ttu-id="cb6fe-126">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-126">This element is optional.</span></span> <span data-ttu-id="cb6fe-127">Se esse elemento não estiver presente, o usuário autenticado será considerado como o remetente.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="cb6fe-128">O elemento **agindo** deve ser incluído para solicitar dicas de remetente.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="cb6fe-129">Um erro **ErrorInvalidArgument** pode ser retornado em uma resposta se o elemento **agindo** estiver ausente, não incluir um tipo de roteamento, não incluir um endereço de email, contiver um endereço de email inválido, não resolver para um usuário nos serviços de domínio do Active Directory (AD DS) ou resolver para vários usuários no AD DS.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="cb6fe-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb6fe-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb6fe-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cb6fe-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb6fe-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb6fe-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb6fe-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cb6fe-133">Schema Name</span></span>  <br/> |<span data-ttu-id="cb6fe-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cb6fe-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb6fe-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cb6fe-135">Validation File</span></span>  <br/> |<span data-ttu-id="cb6fe-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cb6fe-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb6fe-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cb6fe-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb6fe-138">False</span><span class="sxs-lookup"><span data-stu-id="cb6fe-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb6fe-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb6fe-139">See also</span></span>

- [<span data-ttu-id="cb6fe-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cb6fe-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

