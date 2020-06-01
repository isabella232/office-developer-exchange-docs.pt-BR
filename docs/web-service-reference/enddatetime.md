---
title: EndDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateTime
api_type:
- schema
ms.assetid: 54d14e47-a8f7-400b-a859-c7ea7ce4c6a4
description: O elemento EndDateTime especifica a data e hora de término de uma regra ou de uma pesquisa.
ms.openlocfilehash: 9556e4c1ef405ae66a71d19d99d9a71a61f54efc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460131"
---
# <a name="enddatetime"></a><span data-ttu-id="b2701-103">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="b2701-103">EndDateTime</span></span>

<span data-ttu-id="b2701-104">O elemento **EndDateTime** especifica a data e hora de término de uma regra ou de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b2701-104">The **EndDateTime** element specifies the end date and time for a rule or a search.</span></span> 
  
```XML
<EndDateTime/>
```

 <span data-ttu-id="b2701-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b2701-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2701-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b2701-106">Attributes and elements</span></span>

<span data-ttu-id="b2701-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b2701-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2701-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b2701-108">Attributes</span></span>

<span data-ttu-id="b2701-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2701-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2701-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b2701-110">Child elements</span></span>

<span data-ttu-id="b2701-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b2701-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2701-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b2701-112">Parent elements</span></span>

|<span data-ttu-id="b2701-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2701-113">**Element**</span></span>|<span data-ttu-id="b2701-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2701-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2701-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b2701-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b2701-116">Contém critérios para os tipos de mensagens a serem localizados.</span><span class="sxs-lookup"><span data-stu-id="b2701-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b2701-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b2701-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="b2701-118">Especifica o intervalo de datas no qual as mensagens de entrada precisam ser recebidas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="b2701-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2701-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b2701-119">Text value</span></span>

<span data-ttu-id="b2701-120">Um valor de texto que representa uma data/hora será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="b2701-120">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2701-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2701-121">Remarks</span></span>

<span data-ttu-id="b2701-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2701-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2701-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b2701-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2701-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2701-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b2701-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b2701-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b2701-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b2701-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b2701-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b2701-127">Validation File</span></span>  <br/> |<span data-ttu-id="b2701-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b2701-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b2701-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b2701-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2701-130">False</span><span class="sxs-lookup"><span data-stu-id="b2701-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2701-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2701-131">See also</span></span>



- [<span data-ttu-id="b2701-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2701-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

