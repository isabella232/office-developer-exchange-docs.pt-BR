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
description: O elemento GetUserConfiguration representa uma solicitação para obter um objeto de configuração do usuário.
ms.openlocfilehash: 46a2a5ebbabfc038692a5de83e0a960e05295061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457708"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="a7cc3-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7cc3-103">GetUserConfiguration</span></span>

<span data-ttu-id="a7cc3-104">O elemento **GetUserConfiguration** representa uma solicitação para obter um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="a7cc3-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="a7cc3-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7cc3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a7cc3-106">Attributes and elements</span></span>

<span data-ttu-id="a7cc3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7cc3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7cc3-108">Attributes</span></span>

<span data-ttu-id="a7cc3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7cc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7cc3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7cc3-110">Child elements</span></span>

|<span data-ttu-id="a7cc3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7cc3-111">**Element**</span></span>|<span data-ttu-id="a7cc3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7cc3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7cc3-113">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="a7cc3-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="a7cc3-114">Representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="a7cc3-115">Esse elemento deve estar presente em uma solicitação GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="a7cc3-116">Userconfigurationproperties</span><span class="sxs-lookup"><span data-stu-id="a7cc3-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="a7cc3-117">Especifica os tipos de propriedade de configuração do usuário a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="a7cc3-118">Esse elemento deve estar presente em uma solicitação GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7cc3-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7cc3-119">Parent elements</span></span>

<span data-ttu-id="a7cc3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7cc3-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a7cc3-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a7cc3-121">Text value</span></span>

<span data-ttu-id="a7cc3-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a7cc3-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a7cc3-123">Remarks</span></span>

<span data-ttu-id="a7cc3-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7cc3-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7cc3-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a7cc3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7cc3-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7cc3-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a7cc3-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7cc3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a7cc3-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a7cc3-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a7cc3-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7cc3-129">Validation File</span></span>  <br/> |<span data-ttu-id="a7cc3-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a7cc3-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a7cc3-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7cc3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7cc3-132">False</span><span class="sxs-lookup"><span data-stu-id="a7cc3-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7cc3-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="a7cc3-133">See also</span></span>



- [<span data-ttu-id="a7cc3-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a7cc3-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

