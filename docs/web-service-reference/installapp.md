---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: O elemento InstallApp Especifica a solicitação para instalar um aplicativo.
ms.openlocfilehash: d9b7412865c003b89eccbdd92aa6ff9968048191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823949"
---
# <a name="installapp"></a><span data-ttu-id="3a0fc-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="3a0fc-103">InstallApp</span></span>

<span data-ttu-id="3a0fc-104">O elemento **InstallApp** Especifica a solicitação para instalar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="3a0fc-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="3a0fc-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a0fc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3a0fc-106">Attributes and elements</span></span>

<span data-ttu-id="3a0fc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a0fc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a0fc-108">Attributes</span></span>

<span data-ttu-id="3a0fc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a0fc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a0fc-110">Child elements</span></span>

|<span data-ttu-id="3a0fc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3a0fc-111">**Element**</span></span>|<span data-ttu-id="3a0fc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3a0fc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a0fc-113">Manifesto</span><span class="sxs-lookup"><span data-stu-id="3a0fc-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="3a0fc-114">Contém o arquivo de manifesto do aplicativo codificado na base64.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a0fc-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a0fc-115">Parent elements</span></span>

<span data-ttu-id="3a0fc-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a0fc-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a0fc-117">Remarks</span></span>

<span data-ttu-id="3a0fc-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a0fc-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a0fc-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a0fc-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3a0fc-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a0fc-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a0fc-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a0fc-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a0fc-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3a0fc-123">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="3a0fc-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="3a0fc-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a0fc-124">Validation File</span></span>  <br/> |<span data-ttu-id="3a0fc-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a0fc-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a0fc-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3a0fc-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3a0fc-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="3a0fc-127">See also</span></span>



- [<span data-ttu-id="3a0fc-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3a0fc-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

