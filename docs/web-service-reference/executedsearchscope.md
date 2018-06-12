---
title: ExecutedSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExecutedSearchScope
api_type:
- schema
ms.assetid: 2de5f0ad-43f2-4d38-b520-06540066564e
description: O elemento ExecutedSearchScope contém o escopo da pesquisa que foi executada para obter os resultados da pesquisa.
ms.openlocfilehash: ece9fdfc156cedad2a9fa181897145ae4eea20a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752135"
---
# <a name="executedsearchscope"></a><span data-ttu-id="f593a-103">ExecutedSearchScope</span><span class="sxs-lookup"><span data-stu-id="f593a-103">ExecutedSearchScope</span></span>

<span data-ttu-id="f593a-104">O elemento **ExecutedSearchScope** contém o escopo da pesquisa que foi executada para obter os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f593a-104">The **ExecutedSearchScope** element contains the scope of the search that was performed to get the search results.</span></span> 
  
```xml
<ExecutedSearchScope/>
```

 <span data-ttu-id="f593a-105">**String**</span><span class="sxs-lookup"><span data-stu-id="f593a-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f593a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f593a-106">Attributes and elements</span></span>

<span data-ttu-id="f593a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f593a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f593a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f593a-108">Attributes</span></span>

<span data-ttu-id="f593a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f593a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f593a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f593a-110">Child elements</span></span>

<span data-ttu-id="f593a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f593a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f593a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f593a-112">Parent elements</span></span>

|<span data-ttu-id="f593a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f593a-113">**Element**</span></span>|<span data-ttu-id="f593a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f593a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f593a-115">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="f593a-115">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="f593a-116">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f593a-116">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f593a-117">Text value</span><span class="sxs-lookup"><span data-stu-id="f593a-117">Text value</span></span>

<span data-ttu-id="f593a-118">O valor de texto é opcional.</span><span class="sxs-lookup"><span data-stu-id="f593a-118">The text value is optional.</span></span> <span data-ttu-id="f593a-119">Essa informação é usada pelo aplicativo cliente para armazenar em cache os resultados com mais eficiência.</span><span class="sxs-lookup"><span data-stu-id="f593a-119">This information is used by the client application to cache the results more effectively.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f593a-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f593a-120">Remarks</span></span>

<span data-ttu-id="f593a-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f593a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f593a-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f593a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f593a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f593a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f593a-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f593a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f593a-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f593a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f593a-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f593a-126">Validation File</span></span>  <br/> |<span data-ttu-id="f593a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f593a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f593a-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f593a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f593a-129">False</span><span class="sxs-lookup"><span data-stu-id="f593a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f593a-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="f593a-130">See also</span></span>



[<span data-ttu-id="f593a-131">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f593a-131">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="f593a-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f593a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

