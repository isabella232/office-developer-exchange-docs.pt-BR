---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: O elemento ServerVersionInfo contém a versão do servidor que processou a solicitação.
ms.openlocfilehash: b54b4833361ec78c7f8213473af4638965c7ddae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467645"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="33c74-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="33c74-104">O elemento **ServerVersionInfo** contém a versão do servidor que processou a solicitação.</span><span class="sxs-lookup"><span data-stu-id="33c74-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="33c74-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="33c74-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33c74-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="33c74-106">Attributes and elements</span></span>

<span data-ttu-id="33c74-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="33c74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33c74-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="33c74-108">Attributes</span></span>

<span data-ttu-id="33c74-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33c74-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="33c74-110">Child elements</span></span>

|<span data-ttu-id="33c74-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="33c74-111">**Element**</span></span>|<span data-ttu-id="33c74-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33c74-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33c74-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="33c74-114">O número da versão principal do servidor.</span><span class="sxs-lookup"><span data-stu-id="33c74-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="33c74-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="33c74-116">O número da versão secundária do servidor.</span><span class="sxs-lookup"><span data-stu-id="33c74-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="33c74-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="33c74-118">O número de compilação principal do servidor.</span><span class="sxs-lookup"><span data-stu-id="33c74-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="33c74-119">MinorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="33c74-120">O número de compilação secundário para o servidor.</span><span class="sxs-lookup"><span data-stu-id="33c74-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="33c74-121">Versão (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33c74-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="33c74-122">Uma descrição da versão do produto do servidor.</span><span class="sxs-lookup"><span data-stu-id="33c74-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33c74-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="33c74-123">Parent elements</span></span>

<span data-ttu-id="33c74-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c74-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33c74-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="33c74-125">Remarks</span></span>

<span data-ttu-id="33c74-126">Este elemento é retornado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="33c74-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33c74-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="33c74-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33c74-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="33c74-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="33c74-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="33c74-129">Schema Name</span></span>  <br/> |<span data-ttu-id="33c74-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33c74-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="33c74-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="33c74-131">Validation File</span></span>  <br/> |<span data-ttu-id="33c74-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33c74-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33c74-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="33c74-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="33c74-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="33c74-134">True</span></span>  <br/> |
   

