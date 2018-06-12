---
title: DeleteUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 91b18b6a-d904-476c-996d-b041e859da1e
description: O elemento DeleteUserConfiguration representa uma solicitação para excluir um objeto de configuração do usuário.
ms.openlocfilehash: e357c32f95cddc866b77b6f1172ab260837b061b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751757"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="d4e21-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4e21-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="d4e21-104">O elemento **DeleteUserConfiguration** representa uma solicitação para excluir um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4e21-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="d4e21-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="d4e21-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4e21-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d4e21-106">Attributes and elements</span></span>

<span data-ttu-id="d4e21-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d4e21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4e21-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d4e21-108">Attributes</span></span>

<span data-ttu-id="d4e21-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4e21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4e21-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d4e21-110">Child elements</span></span>

|<span data-ttu-id="d4e21-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4e21-111">**Element**</span></span>|<span data-ttu-id="d4e21-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4e21-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4e21-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="d4e21-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="d4e21-114">Representa o nome do objeto de configuração do usuário para excluir.</span><span class="sxs-lookup"><span data-stu-id="d4e21-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4e21-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d4e21-115">Parent elements</span></span>

<span data-ttu-id="d4e21-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4e21-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d4e21-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d4e21-117">Text value</span></span>

<span data-ttu-id="d4e21-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d4e21-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4e21-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="d4e21-119">Remarks</span></span>

<span data-ttu-id="d4e21-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4e21-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4e21-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d4e21-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4e21-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4e21-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4e21-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d4e21-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d4e21-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d4e21-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4e21-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d4e21-125">Validation File</span></span>  <br/> |<span data-ttu-id="d4e21-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4e21-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4e21-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d4e21-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4e21-128">False</span><span class="sxs-lookup"><span data-stu-id="d4e21-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4e21-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="d4e21-129">See also</span></span>

- [<span data-ttu-id="d4e21-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d4e21-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

