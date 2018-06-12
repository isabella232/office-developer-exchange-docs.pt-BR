---
title: ReportTemplate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: O elemento ReportTemplate representa o tipo de relatório a ser obtido.
ms.openlocfilehash: 70aab69f4d20ad9fd7e878c7fccd16e261c9b94c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825118"
---
# <a name="reporttemplate"></a><span data-ttu-id="e9aba-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="e9aba-103">ReportTemplate</span></span>

<span data-ttu-id="e9aba-104">O elemento **ReportTemplate** representa o tipo de relatório a ser obtido.</span><span class="sxs-lookup"><span data-stu-id="e9aba-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="e9aba-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="e9aba-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9aba-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e9aba-106">Attributes and elements</span></span>

<span data-ttu-id="e9aba-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e9aba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9aba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e9aba-108">Attributes</span></span>

<span data-ttu-id="e9aba-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9aba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9aba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e9aba-110">Child elements</span></span>

<span data-ttu-id="e9aba-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e9aba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9aba-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e9aba-112">Parent elements</span></span>

|<span data-ttu-id="e9aba-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e9aba-113">**Element**</span></span>|<span data-ttu-id="e9aba-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e9aba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9aba-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e9aba-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="e9aba-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="e9aba-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e9aba-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e9aba-117">Text value</span></span>

<span data-ttu-id="e9aba-118">A tabela a seguir lista os valores possíveis para o elemento **ReportTemplate** .</span><span class="sxs-lookup"><span data-stu-id="e9aba-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="e9aba-119">**Valores de elemento ReportTemplate**</span><span class="sxs-lookup"><span data-stu-id="e9aba-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="e9aba-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e9aba-120">**Value**</span></span>|<span data-ttu-id="e9aba-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e9aba-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e9aba-122">Resumo</span><span class="sxs-lookup"><span data-stu-id="e9aba-122">Summary</span></span>  <br/> |<span data-ttu-id="e9aba-123">Especifica que o relatório exibirá todos os destinatários da mensagem e o status de entrega da mensagem para cada destinatário.</span><span class="sxs-lookup"><span data-stu-id="e9aba-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="e9aba-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="e9aba-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="e9aba-125">Especifica que, para um único destinatário, o relatório exibirá um histórico completo dos eventos que ocorreram.</span><span class="sxs-lookup"><span data-stu-id="e9aba-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9aba-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e9aba-126">Remarks</span></span>

<span data-ttu-id="e9aba-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e9aba-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9aba-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e9aba-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9aba-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9aba-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9aba-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e9aba-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e9aba-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e9aba-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9aba-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e9aba-132">Validation File</span></span>  <br/> |<span data-ttu-id="e9aba-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e9aba-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9aba-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e9aba-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9aba-135">False</span><span class="sxs-lookup"><span data-stu-id="e9aba-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9aba-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="e9aba-136">See also</span></span>



- [<span data-ttu-id="e9aba-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e9aba-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

