---
title: GetDiscoverySearchConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d963e6c-e94d-462b-8c44-95d55c848fb2
description: O elemento GetDiscoverySearchConfigurationResponse especifica a resposta a uma solicitação GetDiscoverySearchConfiguration.
ms.openlocfilehash: 98393943434b5e3460485b7d75c2b5285983f597
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460978"
---
# <a name="getdiscoverysearchconfigurationresponse"></a><span data-ttu-id="01918-103">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="01918-103">GetDiscoverySearchConfigurationResponse</span></span>

<span data-ttu-id="01918-104">O elemento **GetDiscoverySearchConfigurationResponse** especifica a resposta a uma solicitação **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="01918-104">The **GetDiscoverySearchConfigurationResponse** element specifies the response to a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 <span data-ttu-id="01918-105">**GetDiscoverySearchConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="01918-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01918-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="01918-106">Attributes and elements</span></span>

<span data-ttu-id="01918-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01918-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01918-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01918-108">Attributes</span></span>

<span data-ttu-id="01918-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01918-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01918-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01918-110">Child elements</span></span>

<span data-ttu-id="01918-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="01918-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01918-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01918-112">Parent elements</span></span>

[<span data-ttu-id="01918-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01918-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="01918-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="01918-114">Remarks</span></span>

<span data-ttu-id="01918-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="01918-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01918-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01918-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01918-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="01918-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01918-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="01918-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01918-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01918-119">Schema name</span></span>  <br/> |<span data-ttu-id="01918-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="01918-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01918-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01918-121">Validation file</span></span>  <br/> |<span data-ttu-id="01918-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01918-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01918-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="01918-123">Can be empty</span></span>  <br/> |<span data-ttu-id="01918-124">falso</span><span class="sxs-lookup"><span data-stu-id="01918-124">false</span></span>  <br/> |
   

