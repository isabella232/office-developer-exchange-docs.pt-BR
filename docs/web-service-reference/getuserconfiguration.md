---
title: GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 4044c0a1-cd88-41ae-9cc4-a7cf2b279094
description: O elemento GetUserConfiguration representam uma solicitação para obter um objeto de configuração do usuário.
ms.openlocfilehash: 81f2ca4995de69d6547412ec699a2ceaddcce385
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823688"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="08f73-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f73-103">GetUserConfiguration</span></span>

<span data-ttu-id="08f73-104">O elemento **GetUserConfiguration** representam uma solicitação para obter um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="08f73-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="08f73-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="08f73-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08f73-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="08f73-106">Attributes and elements</span></span>

<span data-ttu-id="08f73-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="08f73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08f73-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="08f73-108">Attributes</span></span>

<span data-ttu-id="08f73-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="08f73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08f73-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="08f73-110">Child elements</span></span>

|<span data-ttu-id="08f73-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="08f73-111">**Element**</span></span>|<span data-ttu-id="08f73-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="08f73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08f73-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="08f73-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="08f73-114">Representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="08f73-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="08f73-115">Este elemento deve estar presente em uma solicitação de GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="08f73-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="08f73-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="08f73-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="08f73-117">Especifica os tipos de propriedade de configuração do usuário para retornar.</span><span class="sxs-lookup"><span data-stu-id="08f73-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="08f73-118">Este elemento deve estar presente em uma solicitação de GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="08f73-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08f73-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="08f73-119">Parent elements</span></span>

<span data-ttu-id="08f73-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="08f73-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="08f73-121">Text value</span><span class="sxs-lookup"><span data-stu-id="08f73-121">Text value</span></span>

<span data-ttu-id="08f73-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="08f73-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08f73-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="08f73-123">Remarks</span></span>

<span data-ttu-id="08f73-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="08f73-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08f73-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="08f73-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08f73-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="08f73-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08f73-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="08f73-127">Schema Name</span></span>  <br/> |<span data-ttu-id="08f73-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="08f73-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="08f73-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="08f73-129">Validation File</span></span>  <br/> |<span data-ttu-id="08f73-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="08f73-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08f73-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="08f73-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="08f73-132">False</span><span class="sxs-lookup"><span data-stu-id="08f73-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08f73-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="08f73-133">See also</span></span>



- [<span data-ttu-id="08f73-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="08f73-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

