---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: O elemento GetServiceConfiguration define uma solicitação GetServiceConfiguration.
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457869"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="3dd3e-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dd3e-103">GetServiceConfiguration</span></span>

<span data-ttu-id="3dd3e-104">O elemento **GetServiceConfiguration** define uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="3dd3e-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="3dd3e-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dd3e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3dd3e-106">Attributes and elements</span></span>

<span data-ttu-id="3dd3e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dd3e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3dd3e-108">Attributes</span></span>

<span data-ttu-id="3dd3e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dd3e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dd3e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3dd3e-110">Child elements</span></span>

|<span data-ttu-id="3dd3e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3dd3e-111">**Element**</span></span>|<span data-ttu-id="3dd3e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3dd3e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dd3e-113">Agindo</span><span class="sxs-lookup"><span data-stu-id="3dd3e-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="3dd3e-114">Identifica quem o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="3dd3e-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-115">This element is optional.</span></span> <span data-ttu-id="3dd3e-116">Se esse elemento não estiver presente, o usuário autenticado será considerado como o remetente.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="3dd3e-117">O elemento **agindo** deve ser incluído para solicitar dicas de remetente.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="3dd3e-118">Um erro ErrorInvalidArgument pode ser retornado em uma resposta se o elemento **agindo** estiver ausente, não incluir um tipo de roteamento, não incluir um endereço de email, contiver um endereço de email inválido, não resolver para um usuário nos serviços de domínio do Active Directory (AD DS) ou resolver para vários usuários no AD DS.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="3dd3e-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dd3e-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="3dd3e-120">Contém as configurações de serviço solicitadas.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-120">Contains the requested service configurations.</span></span> <span data-ttu-id="3dd3e-121">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3dd3e-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3dd3e-122">Parent elements</span></span>

<span data-ttu-id="3dd3e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dd3e-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3dd3e-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3dd3e-124">Text value</span></span>

<span data-ttu-id="3dd3e-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3dd3e-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="3dd3e-126">Remarks</span></span>

<span data-ttu-id="3dd3e-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3dd3e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dd3e-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3dd3e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dd3e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dd3e-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3dd3e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3dd3e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3dd3e-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3dd3e-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3dd3e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3dd3e-132">Validation File</span></span>  <br/> |<span data-ttu-id="3dd3e-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3dd3e-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dd3e-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3dd3e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dd3e-135">False</span><span class="sxs-lookup"><span data-stu-id="3dd3e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dd3e-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="3dd3e-136">See also</span></span>



- [<span data-ttu-id="3dd3e-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3dd3e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

