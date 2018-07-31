---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: O elemento de GetAppManifestsResponse define a resposta a uma solicitação de operação GetAppManifests.
ms.openlocfilehash: ae9d1d853023a5b42db2e8fee2ed57f585433f69
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354145"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="194e6-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="194e6-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="194e6-104">O elemento de **GetAppManifestsResponse** define a resposta a uma solicitação de operação **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="194e6-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Apps/>
</GetAppManifestsResponse>
```

<span data-ttu-id="194e6-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="194e6-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="194e6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="194e6-106">Attributes and elements</span></span>

<span data-ttu-id="194e6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="194e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="194e6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="194e6-108">Attributes</span></span>

<span data-ttu-id="194e6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="194e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="194e6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="194e6-110">Child elements</span></span>

<span data-ttu-id="194e6-111">[ResponseCode](responsecode.md) | [manifestos](manifests.md) | [Apps](apps.md)</span><span class="sxs-lookup"><span data-stu-id="194e6-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="194e6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="194e6-112">Parent elements</span></span>

<span data-ttu-id="194e6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="194e6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="194e6-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="194e6-114">Remarks</span></span>

<span data-ttu-id="194e6-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="194e6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="194e6-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="194e6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="194e6-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="194e6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="194e6-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="194e6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="194e6-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="194e6-119">Schema Name</span></span>  <br/> |<span data-ttu-id="194e6-120">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="194e6-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="194e6-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="194e6-121">Validation File</span></span>  <br/> |<span data-ttu-id="194e6-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="194e6-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="194e6-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="194e6-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="194e6-124">False</span><span class="sxs-lookup"><span data-stu-id="194e6-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="194e6-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="194e6-125">See also</span></span>

- [<span data-ttu-id="194e6-126">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="194e6-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

