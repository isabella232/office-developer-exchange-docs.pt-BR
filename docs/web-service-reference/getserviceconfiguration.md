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
description: O elemento de GetServiceConfiguration define uma solicitação GetServiceConfiguration.
ms.openlocfilehash: 7ff7124ff062f21a02fc69b86b7cc7367ba3fcb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823666"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="755f8-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="755f8-103">GetServiceConfiguration</span></span>

<span data-ttu-id="755f8-104">O elemento de **GetServiceConfiguration** define uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="755f8-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="755f8-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="755f8-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="755f8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="755f8-106">Attributes and elements</span></span>

<span data-ttu-id="755f8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="755f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="755f8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="755f8-108">Attributes</span></span>

<span data-ttu-id="755f8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="755f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="755f8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="755f8-110">Child elements</span></span>

|<span data-ttu-id="755f8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="755f8-111">**Element**</span></span>|<span data-ttu-id="755f8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="755f8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="755f8-113">ActingAs</span><span class="sxs-lookup"><span data-stu-id="755f8-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="755f8-114">Identifica que o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="755f8-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="755f8-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="755f8-115">This element is optional.</span></span> <span data-ttu-id="755f8-116">Se esse elemento não estiver presente, o usuário autenticado é considerado o remetente.</span><span class="sxs-lookup"><span data-stu-id="755f8-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="755f8-117">O elemento **ActingAs** deve ser incluído para solicitar as dicas de remetente.</span><span class="sxs-lookup"><span data-stu-id="755f8-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="755f8-118">Pode ser retornado um erro de ErrorInvalidArgument em uma resposta, se o elemento **ActingAs** está ausente, não incluir um tipo de roteamento, não inclue um endereço de email, contém um endereço de email inválido, não é resolvido para um usuário no domínio do Active Directory Serviços (AD DS) ou resolva a vários usuários no AD DS.</span><span class="sxs-lookup"><span data-stu-id="755f8-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="755f8-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="755f8-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="755f8-120">Contém as configurações do serviço solicitado.</span><span class="sxs-lookup"><span data-stu-id="755f8-120">Contains the requested service configurations.</span></span> <span data-ttu-id="755f8-121">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="755f8-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="755f8-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="755f8-122">Parent elements</span></span>

<span data-ttu-id="755f8-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="755f8-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="755f8-124">Text value</span><span class="sxs-lookup"><span data-stu-id="755f8-124">Text value</span></span>

<span data-ttu-id="755f8-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="755f8-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="755f8-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="755f8-126">Remarks</span></span>

<span data-ttu-id="755f8-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="755f8-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="755f8-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="755f8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="755f8-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="755f8-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="755f8-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="755f8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="755f8-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="755f8-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="755f8-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="755f8-132">Validation File</span></span>  <br/> |<span data-ttu-id="755f8-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="755f8-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="755f8-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="755f8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="755f8-135">False</span><span class="sxs-lookup"><span data-stu-id="755f8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="755f8-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="755f8-136">See also</span></span>



- [<span data-ttu-id="755f8-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="755f8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

