---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: O elemento DisableApp especifica uma solicitação para desabilitar um aplicativo.
ms.openlocfilehash: e99464677dc34e011e45548083fb830b819649fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457820"
---
# <a name="disableapp"></a><span data-ttu-id="27c37-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="27c37-103">DisableApp</span></span>

<span data-ttu-id="27c37-104">O elemento **DisableApp** especifica uma solicitação para desabilitar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27c37-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="27c37-105">**DisableAppType**</span><span class="sxs-lookup"><span data-stu-id="27c37-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27c37-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="27c37-106">Attributes and elements</span></span>

<span data-ttu-id="27c37-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="27c37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27c37-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="27c37-108">Attributes</span></span>

<span data-ttu-id="27c37-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27c37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27c37-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="27c37-110">Child elements</span></span>

|<span data-ttu-id="27c37-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="27c37-111">**Element**</span></span>|<span data-ttu-id="27c37-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="27c37-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27c37-113">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="27c37-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="27c37-114">Especifica o identificador de um item.</span><span class="sxs-lookup"><span data-stu-id="27c37-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="27c37-115">DisableReason</span><span class="sxs-lookup"><span data-stu-id="27c37-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="27c37-116">Especifica o motivo para desabilitar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27c37-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27c37-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="27c37-117">Parent elements</span></span>

<span data-ttu-id="27c37-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27c37-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27c37-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="27c37-119">Remarks</span></span>

<span data-ttu-id="27c37-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="27c37-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="27c37-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="27c37-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27c37-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="27c37-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27c37-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="27c37-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27c37-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="27c37-124">Schema Name</span></span>  <br/> |<span data-ttu-id="27c37-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="27c37-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="27c37-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="27c37-126">Validation File</span></span>  <br/> |<span data-ttu-id="27c37-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="27c37-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27c37-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="27c37-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="27c37-129">Também consulte</span><span class="sxs-lookup"><span data-stu-id="27c37-129">See also</span></span>

- [<span data-ttu-id="27c37-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="27c37-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

