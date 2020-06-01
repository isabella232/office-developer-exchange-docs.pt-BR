---
title: Userconfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: O elemento userconfiguration define um único objeto de configuração do usuário.
ms.openlocfilehash: 1217f5d591570c2d8df49a116b6bf35c243d1e0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468905"
---
# <a name="userconfiguration"></a><span data-ttu-id="4ef68-103">Userconfiguration</span><span class="sxs-lookup"><span data-stu-id="4ef68-103">UserConfiguration</span></span>

<span data-ttu-id="4ef68-104">O elemento **userconfiguration** define um único objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="4ef68-105">**Userconfigurationtype**</span><span class="sxs-lookup"><span data-stu-id="4ef68-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ef68-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ef68-106">Attributes and elements</span></span>

<span data-ttu-id="4ef68-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ef68-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ef68-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ef68-108">Attributes</span></span>

<span data-ttu-id="4ef68-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ef68-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ef68-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ef68-110">Child elements</span></span>

|<span data-ttu-id="4ef68-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ef68-111">**Element**</span></span>|<span data-ttu-id="4ef68-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ef68-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ef68-113">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="4ef68-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="4ef68-114">Representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="4ef68-115">Este elemento deve ser usado quando você cria um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="4ef68-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4ef68-117">Define o identificador do item de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-118">Dictionary</span><span class="sxs-lookup"><span data-stu-id="4ef68-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="4ef68-119">Define um conjunto de entradas de propriedades de dicionário para um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-120">Nota XMLDATA</span><span class="sxs-lookup"><span data-stu-id="4ef68-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="4ef68-121">Contém o conteúdo da propriedade de dados XML para um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="4ef68-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="4ef68-123">Contém conteúdo de propriedade de dados binários para um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ef68-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ef68-124">Parent elements</span></span>

|<span data-ttu-id="4ef68-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ef68-125">**Element**</span></span>|<span data-ttu-id="4ef68-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ef68-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ef68-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ef68-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="4ef68-128">Representa uma solicitação para criar um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4ef68-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="4ef68-130">Representa uma resposta que retorna um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="4ef68-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ef68-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="4ef68-132">Representa uma solicitação para atualizar um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ef68-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ef68-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ef68-133">Remarks</span></span>

<span data-ttu-id="4ef68-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ef68-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ef68-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4ef68-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ef68-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ef68-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ef68-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ef68-137">Schema Name</span></span>  <br/> |<span data-ttu-id="4ef68-138">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4ef68-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4ef68-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ef68-139">Validation File</span></span>  <br/> |<span data-ttu-id="4ef68-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4ef68-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ef68-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4ef68-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ef68-142">False</span><span class="sxs-lookup"><span data-stu-id="4ef68-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ef68-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ef68-143">See also</span></span>



- [<span data-ttu-id="4ef68-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ef68-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

