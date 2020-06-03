---
title: CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: 43e12e8b-5629-4f5f-9cbd-a99084d8460f
description: O elemento CreateUserConfiguration representa uma solicitação para criar um objeto de configuração do usuário.
ms.openlocfilehash: 1d9194baf309936cb4be088a7ff56250dfa349cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463773"
---
# <a name="createuserconfiguration"></a><span data-ttu-id="ca804-103">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca804-103">CreateUserConfiguration</span></span>

<span data-ttu-id="ca804-104">O elemento **CreateUserConfiguration** representa uma solicitação para criar um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="ca804-104">The **CreateUserConfiguration** element represents a request to create a user configuration object.</span></span> 
  
```xml
<CreateUserConfiguration>
   <UserConfiguration/>
</CreateUserConfiguration>
```

 <span data-ttu-id="ca804-105">**CreateUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="ca804-105">**CreateUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca804-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ca804-106">Attributes and elements</span></span>

<span data-ttu-id="ca804-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ca804-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca804-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ca804-108">Attributes</span></span>

<span data-ttu-id="ca804-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca804-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca804-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ca804-110">Child elements</span></span>

|<span data-ttu-id="ca804-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca804-111">**Element**</span></span>|<span data-ttu-id="ca804-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca804-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca804-113">Userconfiguration</span><span class="sxs-lookup"><span data-stu-id="ca804-113">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="ca804-114">Representa um único objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="ca804-114">Represents a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca804-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ca804-115">Parent elements</span></span>

<span data-ttu-id="ca804-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca804-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ca804-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ca804-117">Text value</span></span>

<span data-ttu-id="ca804-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ca804-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca804-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca804-119">Remarks</span></span>

<span data-ttu-id="ca804-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca804-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca804-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ca804-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca804-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca804-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ca804-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ca804-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ca804-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ca804-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ca804-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ca804-125">Validation File</span></span>  <br/> |<span data-ttu-id="ca804-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ca804-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ca804-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ca804-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca804-128">False</span><span class="sxs-lookup"><span data-stu-id="ca804-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca804-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca804-129">See also</span></span>



- [<span data-ttu-id="ca804-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ca804-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

