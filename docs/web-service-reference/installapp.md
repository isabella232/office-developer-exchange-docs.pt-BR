---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: O elemento InstallApp especifica a solicitação para instalar um aplicativo.
ms.openlocfilehash: 003a72507813677484b2d6ee75f8ff577df169e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468002"
---
# <a name="installapp"></a><span data-ttu-id="743f0-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="743f0-103">InstallApp</span></span>

<span data-ttu-id="743f0-104">O elemento **InstallApp** especifica a solicitação para instalar um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="743f0-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="743f0-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="743f0-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="743f0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="743f0-106">Attributes and elements</span></span>

<span data-ttu-id="743f0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="743f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="743f0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="743f0-108">Attributes</span></span>

<span data-ttu-id="743f0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="743f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="743f0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="743f0-110">Child elements</span></span>

|<span data-ttu-id="743f0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="743f0-111">**Element**</span></span>|<span data-ttu-id="743f0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="743f0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="743f0-113">Manifesto</span><span class="sxs-lookup"><span data-stu-id="743f0-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="743f0-114">Contém o arquivo de manifesto de aplicativo codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="743f0-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="743f0-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="743f0-115">Parent elements</span></span>

<span data-ttu-id="743f0-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="743f0-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="743f0-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="743f0-117">Remarks</span></span>

<span data-ttu-id="743f0-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="743f0-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="743f0-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="743f0-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="743f0-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="743f0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="743f0-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="743f0-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="743f0-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="743f0-122">Schema Name</span></span>  <br/> |<span data-ttu-id="743f0-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="743f0-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="743f0-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="743f0-124">Validation File</span></span>  <br/> |<span data-ttu-id="743f0-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="743f0-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="743f0-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="743f0-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="743f0-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="743f0-127">See also</span></span>



- [<span data-ttu-id="743f0-128">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="743f0-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

