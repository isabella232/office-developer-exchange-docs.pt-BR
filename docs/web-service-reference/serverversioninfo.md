---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: O elemento ServerVersionInfo representa o número de versão do Microsoft Exchange Server.
ms.openlocfilehash: 5bd1fbd8fdee584a9d272fa8ab82f2a31c1357fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466826"
---
# <a name="serverversioninfo"></a><span data-ttu-id="0b7c3-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0b7c3-103">ServerVersionInfo</span></span>

<span data-ttu-id="0b7c3-104">O elemento **ServerVersionInfo** representa o número de versão do Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0b7c3-105">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0b7c3-105">Attributes and elements</span></span>

<span data-ttu-id="0b7c3-106">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b7c3-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b7c3-107">Attributes</span></span>

|<span data-ttu-id="0b7c3-108">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="0b7c3-108">**Attribute**</span></span>|<span data-ttu-id="0b7c3-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b7c3-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b7c3-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="0b7c3-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="0b7c3-111">Descreve o número da versão principal.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="0b7c3-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="0b7c3-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="0b7c3-113">Descreve o número da versão secundária.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="0b7c3-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="0b7c3-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="0b7c3-115">Descreve o número de compilação principal.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="0b7c3-116">MinorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="0b7c3-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="0b7c3-117">Descreve o número de compilação secundário.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="0b7c3-118">Versão</span><span class="sxs-lookup"><span data-stu-id="0b7c3-118">Version</span></span>  <br/> |<span data-ttu-id="0b7c3-119">Descreve a versão do esquema dos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="0b7c3-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b7c3-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b7c3-120">Child elements</span></span>

<span data-ttu-id="0b7c3-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b7c3-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b7c3-122">Parent elements</span></span>

<span data-ttu-id="0b7c3-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b7c3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b7c3-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b7c3-124">Remarks</span></span>

<span data-ttu-id="0b7c3-125">Este elemento é retornado no cabeçalho SOAP de uma mensagem de resposta dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="0b7c3-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0b7c3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0b7c3-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0b7c3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b7c3-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b7c3-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b7c3-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b7c3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0b7c3-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0b7c3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b7c3-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b7c3-131">Validation File</span></span>  <br/> |<span data-ttu-id="0b7c3-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0b7c3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b7c3-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0b7c3-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="0b7c3-134">False</span><span class="sxs-lookup"><span data-stu-id="0b7c3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b7c3-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="0b7c3-135">See also</span></span>



- [<span data-ttu-id="0b7c3-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b7c3-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

