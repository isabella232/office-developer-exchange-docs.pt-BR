---
title: La
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: O elemento Diagnostics fornece informações de tempo e desempenho que são usadas para relatórios em um datacenter.
ms.openlocfilehash: 9eb46ef7ceb877372aff9b029190af8c8d8115cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467834"
---
# <a name="diagnostics"></a><span data-ttu-id="71695-103">La</span><span class="sxs-lookup"><span data-stu-id="71695-103">Diagnostics</span></span>

<span data-ttu-id="71695-104">O elemento **Diagnostics** fornece informações de tempo e desempenho que são usadas para relatórios em um datacenter.</span><span class="sxs-lookup"><span data-stu-id="71695-104">The **Diagnostics** element provides timing and performance information that is used for reporting in a DataCenter.</span></span> 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 <span data-ttu-id="71695-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="71695-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71695-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="71695-106">Attributes and elements</span></span>

<span data-ttu-id="71695-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="71695-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71695-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="71695-108">Attributes</span></span>

<span data-ttu-id="71695-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71695-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71695-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="71695-110">Child elements</span></span>

|<span data-ttu-id="71695-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71695-111">**Element**</span></span>|<span data-ttu-id="71695-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71695-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71695-113">String</span><span class="sxs-lookup"><span data-stu-id="71695-113">String</span></span>](string.md) <br/> |<span data-ttu-id="71695-114">Contém uma cadeia de caracteres que é usada por itens, contatos, tarefas e conversas.</span><span class="sxs-lookup"><span data-stu-id="71695-114">Contains a string that is used by items, contacts, tasks, and conversations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71695-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="71695-115">Parent elements</span></span>

|<span data-ttu-id="71695-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71695-116">**Element**</span></span>|<span data-ttu-id="71695-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71695-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71695-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="71695-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="71695-119">Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="71695-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="71695-120">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="71695-120">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="71695-121">Contém a resposta para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="71695-121">Contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71695-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="71695-122">Text value</span></span>

<span data-ttu-id="71695-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="71695-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71695-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="71695-124">Remarks</span></span>

<span data-ttu-id="71695-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="71695-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71695-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="71695-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71695-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="71695-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71695-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="71695-128">Schema Name</span></span>  <br/> |<span data-ttu-id="71695-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="71695-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="71695-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="71695-130">Validation File</span></span>  <br/> |<span data-ttu-id="71695-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="71695-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71695-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="71695-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="71695-133">False</span><span class="sxs-lookup"><span data-stu-id="71695-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71695-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="71695-134">See also</span></span>

- [<span data-ttu-id="71695-135">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="71695-135">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="71695-136">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="71695-136">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="71695-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="71695-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

