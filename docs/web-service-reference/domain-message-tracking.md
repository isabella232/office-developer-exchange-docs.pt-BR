---
title: Domínio (controle de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 4e8e9efa-8885-4ca5-bf90-424e63768dc3
description: O elemento Domain representa o domínio a ser pesquisado.
ms.openlocfilehash: 77da9028766881b9bc633e1b3318cd4d70c6b72f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457022"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="3d75e-103">Domínio (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="3d75e-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="3d75e-104">O elemento **Domain** representa o domínio a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="3d75e-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="3d75e-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="3d75e-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d75e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3d75e-106">Attributes and elements</span></span>

<span data-ttu-id="3d75e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3d75e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d75e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3d75e-108">Attributes</span></span>

<span data-ttu-id="3d75e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d75e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d75e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3d75e-110">Child elements</span></span>

<span data-ttu-id="3d75e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d75e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d75e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3d75e-112">Parent elements</span></span>

|<span data-ttu-id="3d75e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d75e-113">**Element**</span></span>|<span data-ttu-id="3d75e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d75e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d75e-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3d75e-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="3d75e-116">Contém critérios para os tipos de mensagens a serem localizados.</span><span class="sxs-lookup"><span data-stu-id="3d75e-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3d75e-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3d75e-117">Text value</span></span>

<span data-ttu-id="3d75e-118">Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="3d75e-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3d75e-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d75e-119">Remarks</span></span>

<span data-ttu-id="3d75e-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d75e-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d75e-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3d75e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d75e-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d75e-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3d75e-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3d75e-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3d75e-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3d75e-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3d75e-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3d75e-125">Validation File</span></span>  <br/> |<span data-ttu-id="3d75e-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3d75e-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d75e-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3d75e-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d75e-128">False</span><span class="sxs-lookup"><span data-stu-id="3d75e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d75e-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="3d75e-129">See also</span></span>

- [<span data-ttu-id="3d75e-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3d75e-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

