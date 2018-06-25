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
description: O elemento ServerVersionInfo contém a versão do servidor que processaram a solicitação.
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825385"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="06568-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="06568-104">O elemento **ServerVersionInfo** contém a versão do servidor que processaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="06568-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="06568-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="06568-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06568-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="06568-106">Attributes and elements</span></span>

<span data-ttu-id="06568-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06568-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06568-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="06568-108">Attributes</span></span>

<span data-ttu-id="06568-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06568-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06568-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06568-110">Child elements</span></span>

|<span data-ttu-id="06568-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06568-111">**Element**</span></span>|<span data-ttu-id="06568-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06568-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06568-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="06568-114">O número de versão principal para o servidor.</span><span class="sxs-lookup"><span data-stu-id="06568-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="06568-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="06568-116">O número da versão secundária do servidor.</span><span class="sxs-lookup"><span data-stu-id="06568-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="06568-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="06568-118">O número de compilação principais para o servidor.</span><span class="sxs-lookup"><span data-stu-id="06568-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="06568-119">MinorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="06568-120">O número de compilação secundárias para o servidor.</span><span class="sxs-lookup"><span data-stu-id="06568-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="06568-121">Versão (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06568-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="06568-122">Uma descrição da versão do produto de servidor.</span><span class="sxs-lookup"><span data-stu-id="06568-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06568-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06568-123">Parent elements</span></span>

<span data-ttu-id="06568-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06568-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06568-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="06568-125">Remarks</span></span>

<span data-ttu-id="06568-126">Esse elemento é retornado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="06568-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06568-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="06568-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06568-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="06568-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="06568-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06568-129">Schema Name</span></span>  <br/> |<span data-ttu-id="06568-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="06568-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="06568-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06568-131">Validation File</span></span>  <br/> |<span data-ttu-id="06568-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06568-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06568-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="06568-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="06568-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="06568-134">True</span></span>  <br/> |
   

