---
title: LargeAudienceThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LargeAudienceThreshold
api_type:
- schema
ms.assetid: dacd9db7-b8f0-445d-a3d1-3356b8c2bcd1
description: O elemento LargeAudienceThreshold representa o limite grande de audiência para um cliente.
ms.openlocfilehash: 6d85f9eaf8b7723713877d376876461befa92324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466385"
---
# <a name="largeaudiencethreshold"></a><span data-ttu-id="e9674-103">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="e9674-103">LargeAudienceThreshold</span></span>

<span data-ttu-id="e9674-104">O elemento **LargeAudienceThreshold** representa o limite grande de audiência para um cliente.</span><span class="sxs-lookup"><span data-stu-id="e9674-104">The **LargeAudienceThreshold** element represents the large audience threshold for a client.</span></span> 
  
```XML
<LargeAudienceThreshold/>
```

 <span data-ttu-id="e9674-105">**int**</span><span class="sxs-lookup"><span data-stu-id="e9674-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9674-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e9674-106">Attributes and elements</span></span>

<span data-ttu-id="e9674-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e9674-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9674-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e9674-108">Attributes</span></span>

<span data-ttu-id="e9674-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9674-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9674-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e9674-110">Child elements</span></span>

<span data-ttu-id="e9674-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9674-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9674-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e9674-112">Parent elements</span></span>

|<span data-ttu-id="e9674-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e9674-113">**Element**</span></span>|<span data-ttu-id="e9674-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e9674-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9674-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="e9674-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="e9674-116">Contém informações de configuração de serviço para o serviço de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="e9674-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9674-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e9674-117">Text value</span></span>

<span data-ttu-id="e9674-118">O valor de texto é um inteiro que representa o limite de audiência que indica que a mensagem vai para mais de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="e9674-118">The text value is an integer that represents the audience threshold that indicates that the message is going to more than one person.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9674-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="e9674-119">Remarks</span></span>

<span data-ttu-id="e9674-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e9674-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9674-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e9674-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9674-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9674-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9674-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e9674-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e9674-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e9674-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9674-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e9674-125">Validation File</span></span>  <br/> |<span data-ttu-id="e9674-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e9674-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9674-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e9674-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9674-128">False</span><span class="sxs-lookup"><span data-stu-id="e9674-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9674-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="e9674-129">See also</span></span>



- [<span data-ttu-id="e9674-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e9674-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

