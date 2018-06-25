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
ms.openlocfilehash: aff8a6542e2ae6fb1148dd29051b7b33ad90eeff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825389"
---
# <a name="serverversioninfo"></a><span data-ttu-id="152c1-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="152c1-103">ServerVersionInfo</span></span>

<span data-ttu-id="152c1-104">O elemento **ServerVersionInfo** representa o número de versão do Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="152c1-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="152c1-105">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="152c1-105">Attributes and elements</span></span>

<span data-ttu-id="152c1-106">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="152c1-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="152c1-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="152c1-107">Attributes</span></span>

|<span data-ttu-id="152c1-108">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="152c1-108">**Attribute**</span></span>|<span data-ttu-id="152c1-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="152c1-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="152c1-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="152c1-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="152c1-111">Descreve o número de versão principal.</span><span class="sxs-lookup"><span data-stu-id="152c1-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="152c1-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="152c1-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="152c1-113">Descreve o número de versão secundária.</span><span class="sxs-lookup"><span data-stu-id="152c1-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="152c1-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="152c1-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="152c1-115">Descreve o número de compilação principais.</span><span class="sxs-lookup"><span data-stu-id="152c1-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="152c1-116">MinorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="152c1-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="152c1-117">Descreve o número de compilação secundárias.</span><span class="sxs-lookup"><span data-stu-id="152c1-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="152c1-118">Versão</span><span class="sxs-lookup"><span data-stu-id="152c1-118">Version</span></span>  <br/> |<span data-ttu-id="152c1-119">Descreve a versão do esquema de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="152c1-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="152c1-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="152c1-120">Child elements</span></span>

<span data-ttu-id="152c1-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="152c1-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="152c1-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="152c1-122">Parent elements</span></span>

<span data-ttu-id="152c1-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="152c1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="152c1-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="152c1-124">Remarks</span></span>

<span data-ttu-id="152c1-125">Esse elemento é retornado no cabeçalho SOAP de uma mensagem de resposta de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="152c1-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="152c1-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="152c1-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="152c1-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="152c1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="152c1-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="152c1-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="152c1-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="152c1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="152c1-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="152c1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="152c1-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="152c1-131">Validation File</span></span>  <br/> |<span data-ttu-id="152c1-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="152c1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="152c1-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="152c1-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="152c1-134">False</span><span class="sxs-lookup"><span data-stu-id="152c1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="152c1-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="152c1-135">See also</span></span>



- [<span data-ttu-id="152c1-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="152c1-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

