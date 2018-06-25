---
title: Domínio (rastreamento de mensagens)
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
description: O elemento de domínio representa o domínio a ser pesquisado.
ms.openlocfilehash: dc161557b59acc580d918f2e196457714bce4ba9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751910"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="b8383-103">Domínio (rastreamento de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b8383-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="b8383-104">O elemento de **domínio** representa o domínio a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="b8383-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="b8383-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="b8383-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8383-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b8383-106">Attributes and elements</span></span>

<span data-ttu-id="b8383-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8383-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8383-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8383-108">Attributes</span></span>

<span data-ttu-id="b8383-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8383-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8383-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8383-110">Child elements</span></span>

<span data-ttu-id="b8383-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8383-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8383-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8383-112">Parent elements</span></span>

|<span data-ttu-id="b8383-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8383-113">**Element**</span></span>|<span data-ttu-id="b8383-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8383-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8383-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b8383-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b8383-116">Contém os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="b8383-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8383-117">Text value</span><span class="sxs-lookup"><span data-stu-id="b8383-117">Text value</span></span>

<span data-ttu-id="b8383-118">Se este elemento for usado, será necessário um valor de texto que representa uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b8383-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8383-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8383-119">Remarks</span></span>

<span data-ttu-id="b8383-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8383-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8383-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b8383-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8383-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8383-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8383-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8383-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b8383-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b8383-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8383-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8383-125">Validation File</span></span>  <br/> |<span data-ttu-id="b8383-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b8383-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8383-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b8383-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8383-128">False</span><span class="sxs-lookup"><span data-stu-id="b8383-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8383-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="b8383-129">See also</span></span>

- [<span data-ttu-id="b8383-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b8383-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

