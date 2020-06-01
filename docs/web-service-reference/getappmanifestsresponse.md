---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: O elemento GetAppManifestsResponse define a resposta para uma solicitação de operação GetAppManifests.
ms.openlocfilehash: a01f6265d6d534e2f7868b17acf19f0f5d52a01f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462961"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="d02f7-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="d02f7-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="d02f7-104">O elemento **GetAppManifestsResponse** define a resposta para uma solicitação de operação **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="d02f7-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
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

<span data-ttu-id="d02f7-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="d02f7-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d02f7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d02f7-106">Attributes and elements</span></span>

<span data-ttu-id="d02f7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d02f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d02f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d02f7-108">Attributes</span></span>

<span data-ttu-id="d02f7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d02f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d02f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d02f7-110">Child elements</span></span>

<span data-ttu-id="d02f7-111">[ResponseCode](responsecode.md)  |  [Manifestos](manifests.md)  |  [Aplicativos](apps.md)</span><span class="sxs-lookup"><span data-stu-id="d02f7-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d02f7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d02f7-112">Parent elements</span></span>

<span data-ttu-id="d02f7-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d02f7-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d02f7-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d02f7-114">Remarks</span></span>

<span data-ttu-id="d02f7-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d02f7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d02f7-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d02f7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d02f7-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d02f7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d02f7-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d02f7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d02f7-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d02f7-119">Schema Name</span></span>  <br/> |<span data-ttu-id="d02f7-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d02f7-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="d02f7-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d02f7-121">Validation File</span></span>  <br/> |<span data-ttu-id="d02f7-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d02f7-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d02f7-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d02f7-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="d02f7-124">False</span><span class="sxs-lookup"><span data-stu-id="d02f7-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d02f7-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="d02f7-125">See also</span></span>

- [<span data-ttu-id="d02f7-126">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d02f7-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

