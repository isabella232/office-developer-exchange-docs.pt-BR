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
ms.openlocfilehash: 04668ead48e7c321ed7e91cbbeb67c6154c02283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460754"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="9e551-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e551-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="9e551-104">O elemento **DeleteUserConfiguration** representa uma solicitação para excluir um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="9e551-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="9e551-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="9e551-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e551-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9e551-106">Attributes and elements</span></span>

<span data-ttu-id="9e551-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e551-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e551-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e551-108">Attributes</span></span>

<span data-ttu-id="9e551-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e551-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e551-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e551-110">Child elements</span></span>

|<span data-ttu-id="9e551-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9e551-111">**Element**</span></span>|<span data-ttu-id="9e551-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e551-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e551-113">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="9e551-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="9e551-114">Representa o nome do objeto de configuração do usuário a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="9e551-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e551-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e551-115">Parent elements</span></span>

<span data-ttu-id="9e551-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e551-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9e551-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9e551-117">Text value</span></span>

<span data-ttu-id="9e551-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9e551-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e551-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e551-119">Remarks</span></span>

<span data-ttu-id="9e551-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e551-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e551-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9e551-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e551-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e551-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e551-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e551-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9e551-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9e551-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e551-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e551-125">Validation File</span></span>  <br/> |<span data-ttu-id="9e551-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e551-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e551-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9e551-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e551-128">False</span><span class="sxs-lookup"><span data-stu-id="9e551-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e551-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9e551-129">See also</span></span>

- [<span data-ttu-id="9e551-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9e551-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

