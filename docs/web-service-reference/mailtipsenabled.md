---
title: MailTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: O elemento MailTipsEnabled indica se o serviço de dicas de email está disponível.
ms.openlocfilehash: 6be923733f1cbd584010ce5f8ee5b96178d5c2c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468009"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="5513d-103">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="5513d-103">MailTipsEnabled</span></span>

<span data-ttu-id="5513d-104">O elemento **MailTipsEnabled** indica se o serviço de dicas de email está disponível.</span><span class="sxs-lookup"><span data-stu-id="5513d-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="5513d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5513d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5513d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5513d-106">Attributes and elements</span></span>

<span data-ttu-id="5513d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5513d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5513d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5513d-108">Attributes</span></span>

<span data-ttu-id="5513d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5513d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5513d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5513d-110">Child elements</span></span>

<span data-ttu-id="5513d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5513d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5513d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5513d-112">Parent elements</span></span>

|<span data-ttu-id="5513d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5513d-113">**Element**</span></span>|<span data-ttu-id="5513d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5513d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5513d-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="5513d-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="5513d-116">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="5513d-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5513d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5513d-117">Text value</span></span>

<span data-ttu-id="5513d-118">O valor de texto desse elemento será **true** se o serviço de dicas de email estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="5513d-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="5513d-119">O valor será **false** se o serviço de dicas de email não estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="5513d-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5513d-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="5513d-120">Remarks</span></span>

<span data-ttu-id="5513d-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5513d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5513d-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5513d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5513d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5513d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5513d-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5513d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5513d-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5513d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="5513d-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5513d-126">Validation File</span></span>  <br/> |<span data-ttu-id="5513d-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5513d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5513d-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5513d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5513d-129">False</span><span class="sxs-lookup"><span data-stu-id="5513d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5513d-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="5513d-130">See also</span></span>



- [<span data-ttu-id="5513d-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5513d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

