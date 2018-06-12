---
title: ActingAs
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
description: O elemento ActingAs identifica que o chamador está enviando como.
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752220"
---
# <a name="actingas"></a><span data-ttu-id="f48bb-103">ActingAs</span><span class="sxs-lookup"><span data-stu-id="f48bb-103">ActingAs</span></span>

<span data-ttu-id="f48bb-104">O elemento **ActingAs** identifica que o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="f48bb-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="f48bb-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="f48bb-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f48bb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f48bb-106">Attributes and elements</span></span>

<span data-ttu-id="f48bb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f48bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f48bb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f48bb-108">Attributes</span></span>

<span data-ttu-id="f48bb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f48bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f48bb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f48bb-110">Child elements</span></span>

|<span data-ttu-id="f48bb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f48bb-111">**Element**</span></span>|<span data-ttu-id="f48bb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f48bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f48bb-113">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f48bb-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="f48bb-114">Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f48bb-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="f48bb-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f48bb-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f48bb-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f48bb-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="f48bb-117">Define o roteamento que é usado para a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f48bb-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="f48bb-118">O padrão é SMTP.</span><span class="sxs-lookup"><span data-stu-id="f48bb-118">The default is SMTP.</span></span> <span data-ttu-id="f48bb-119">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f48bb-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f48bb-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f48bb-120">Parent elements</span></span>

|<span data-ttu-id="f48bb-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f48bb-121">**Element**</span></span>|<span data-ttu-id="f48bb-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f48bb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f48bb-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f48bb-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="f48bb-124">Define uma solicitação **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="f48bb-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f48bb-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f48bb-125">Remarks</span></span>

<span data-ttu-id="f48bb-126">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f48bb-126">This element is optional.</span></span> <span data-ttu-id="f48bb-127">Se esse elemento não estiver presente, o usuário autenticado é considerado o remetente.</span><span class="sxs-lookup"><span data-stu-id="f48bb-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="f48bb-128">O elemento **ActingAs** deve ser incluído para solicitar as dicas de remetente.</span><span class="sxs-lookup"><span data-stu-id="f48bb-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="f48bb-129">Pode ser retornado um erro de **ErrorInvalidArgument** em uma resposta, se o elemento **ActingAs** está ausente, não incluir um tipo de roteamento, não inclue um endereço de email, contém um endereço de email inválido, não é resolvido para um usuário no Active Directory Serviços de domínio (AD DS) ou resolve para vários usuários no AD DS.</span><span class="sxs-lookup"><span data-stu-id="f48bb-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="f48bb-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f48bb-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f48bb-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f48bb-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f48bb-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f48bb-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f48bb-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f48bb-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f48bb-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f48bb-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f48bb-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f48bb-135">Validation File</span></span>  <br/> |<span data-ttu-id="f48bb-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f48bb-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f48bb-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f48bb-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f48bb-138">False</span><span class="sxs-lookup"><span data-stu-id="f48bb-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f48bb-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="f48bb-139">See also</span></span>

- [<span data-ttu-id="f48bb-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f48bb-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

