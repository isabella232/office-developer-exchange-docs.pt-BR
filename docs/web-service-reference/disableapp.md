---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: O elemento DisableApp Especifica uma solicitação para desabilitar um aplicativo.
ms.openlocfilehash: d6d895d98fb368a6912f9111a4b934ba9631268e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751822"
---
# <a name="disableapp"></a><span data-ttu-id="f7c5d-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="f7c5d-103">DisableApp</span></span>

<span data-ttu-id="f7c5d-104">O elemento **DisableApp** Especifica uma solicitação para desabilitar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="f7c5d-105">**DisableAppType**</span><span class="sxs-lookup"><span data-stu-id="f7c5d-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7c5d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f7c5d-106">Attributes and elements</span></span>

<span data-ttu-id="f7c5d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7c5d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f7c5d-108">Attributes</span></span>

<span data-ttu-id="f7c5d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7c5d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f7c5d-110">Child elements</span></span>

|<span data-ttu-id="f7c5d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7c5d-111">**Element**</span></span>|<span data-ttu-id="f7c5d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7c5d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7c5d-113">ID (String)</span><span class="sxs-lookup"><span data-stu-id="f7c5d-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="f7c5d-114">Especifica o identificador de um item.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="f7c5d-115">DisableReason</span><span class="sxs-lookup"><span data-stu-id="f7c5d-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="f7c5d-116">Especifica a razão para desabilitar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7c5d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f7c5d-117">Parent elements</span></span>

<span data-ttu-id="f7c5d-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7c5d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="f7c5d-119">Remarks</span></span>

<span data-ttu-id="f7c5d-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f7c5d-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7c5d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7c5d-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f7c5d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7c5d-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7c5d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7c5d-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f7c5d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f7c5d-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="f7c5d-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="f7c5d-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f7c5d-126">Validation File</span></span>  <br/> |<span data-ttu-id="f7c5d-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f7c5d-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7c5d-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f7c5d-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f7c5d-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7c5d-129">See also</span></span>

- [<span data-ttu-id="f7c5d-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f7c5d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

