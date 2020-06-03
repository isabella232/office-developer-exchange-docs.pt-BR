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
ms.openlocfilehash: 22f14d326032a30e5cb4c2c9e1aff390d98e95e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528696"
---
# <a name="reporttemplate"></a><span data-ttu-id="f0408-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="f0408-103">ReportTemplate</span></span>

<span data-ttu-id="f0408-104">O elemento **ReportTemplate** representa o tipo de relatório a ser obtido.</span><span class="sxs-lookup"><span data-stu-id="f0408-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="f0408-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="f0408-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0408-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f0408-106">Attributes and elements</span></span>

<span data-ttu-id="f0408-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f0408-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0408-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f0408-108">Attributes</span></span>

<span data-ttu-id="f0408-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0408-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0408-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f0408-110">Child elements</span></span>

<span data-ttu-id="f0408-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f0408-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0408-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f0408-112">Parent elements</span></span>

|<span data-ttu-id="f0408-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f0408-113">**Element**</span></span>|<span data-ttu-id="f0408-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0408-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0408-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f0408-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="f0408-116">Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) para recuperar o relatório de acompanhamento de mensagens completo da ID especificada.</span><span class="sxs-lookup"><span data-stu-id="f0408-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0408-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f0408-117">Text value</span></span>

<span data-ttu-id="f0408-118">A tabela a seguir lista os valores possíveis para o elemento **ReportTemplate** .</span><span class="sxs-lookup"><span data-stu-id="f0408-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="f0408-119">**Valores do elemento ReportTemplate**</span><span class="sxs-lookup"><span data-stu-id="f0408-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="f0408-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f0408-120">**Value**</span></span>|<span data-ttu-id="f0408-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0408-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0408-122">Resumo</span><span class="sxs-lookup"><span data-stu-id="f0408-122">Summary</span></span>  <br/> |<span data-ttu-id="f0408-123">Especifica que o relatório exibirá todos os destinatários da mensagem e o status de entrega da mensagem para cada destinatário.</span><span class="sxs-lookup"><span data-stu-id="f0408-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="f0408-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="f0408-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="f0408-125">Especifica que, para um único destinatário, o relatório exibirá um histórico completo dos eventos que ocorreram.</span><span class="sxs-lookup"><span data-stu-id="f0408-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0408-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0408-126">Remarks</span></span>

<span data-ttu-id="f0408-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f0408-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0408-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f0408-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0408-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="f0408-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0408-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f0408-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f0408-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f0408-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0408-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f0408-132">Validation File</span></span>  <br/> |<span data-ttu-id="f0408-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0408-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0408-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f0408-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0408-135">False</span><span class="sxs-lookup"><span data-stu-id="f0408-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0408-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="f0408-136">See also</span></span>



- [<span data-ttu-id="f0408-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f0408-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

