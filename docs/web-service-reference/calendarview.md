---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: O elemento CalendarView define uma operação FindItem como retornar itens de calendário em um conjunto como eles aparecem em um calendário.
ms.openlocfilehash: e547a4b2db5c09ebefd9a072da6cc4733818002e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462259"
---
# <a name="calendarview"></a><span data-ttu-id="121eb-103">CalendarView</span><span class="sxs-lookup"><span data-stu-id="121eb-103">CalendarView</span></span>

<span data-ttu-id="121eb-104">O elemento **CalendarView** define uma [operação FindItem](finditem-operation.md) como retornar itens de calendário em um conjunto como eles aparecem em um calendário.</span><span class="sxs-lookup"><span data-stu-id="121eb-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="121eb-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="121eb-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="121eb-106">Modo de exibição do Calendário</span><span class="sxs-lookup"><span data-stu-id="121eb-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="121eb-107">**Modo de exibição do Calendário**</span><span class="sxs-lookup"><span data-stu-id="121eb-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="121eb-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="121eb-108">Attributes and elements</span></span>

<span data-ttu-id="121eb-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="121eb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="121eb-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="121eb-110">Attributes</span></span>

|<span data-ttu-id="121eb-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="121eb-111">**Attribute**</span></span>|<span data-ttu-id="121eb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="121eb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="121eb-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="121eb-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="121eb-114">Descreve o número máximo de resultados a serem retornados na resposta FindItem.</span><span class="sxs-lookup"><span data-stu-id="121eb-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="121eb-115">**StartDate**</span><span class="sxs-lookup"><span data-stu-id="121eb-115">**StartDate**</span></span> <br/> |<span data-ttu-id="121eb-116">Identifica o início de um período de tempo consultado para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="121eb-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="121eb-117">Todos os itens de calendário que têm uma hora de término anterior à **StartDate** não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="121eb-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="121eb-118">O valor de **StartDate** pode ser especificado no formato UTC (tempo Universal Coordenado), como em 2006-01-02T12:00:00Z ou em um formato em que o horário local e o deslocamento de fuso horário são especificados, como em 2006-01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="121eb-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="121eb-119">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="121eb-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="121eb-120">**EndDate**</span><span class="sxs-lookup"><span data-stu-id="121eb-120">**EndDate**</span></span> <br/> |<span data-ttu-id="121eb-121">Identifica o final de um período de tempo consultado para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="121eb-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="121eb-122">Todos os itens de calendário que têm um horário de início ou depois de **EndDate** não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="121eb-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="121eb-123">O valor de **EndDate** pode ser especificado no formato UTC, como em 2006-02-02T12:00:00Z ou em um formato em que o horário local e o deslocamento de fuso horário são especificados, como em 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="121eb-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="121eb-124">**EndDate** deve ser maior ou igual a **StartDate**; caso contrário, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="121eb-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="121eb-125">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="121eb-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="121eb-126">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="121eb-126">Child elements</span></span>

<span data-ttu-id="121eb-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="121eb-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="121eb-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="121eb-128">Parent elements</span></span>

|<span data-ttu-id="121eb-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="121eb-129">**Element**</span></span>|<span data-ttu-id="121eb-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="121eb-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="121eb-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="121eb-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="121eb-132">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="121eb-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="121eb-133">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="121eb-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="121eb-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="121eb-134">Remarks</span></span>

<span data-ttu-id="121eb-135">Se o elemento **CalendarView** for especificado em uma solicitação FindItem, o serviço Web retornará uma lista de itens de calendário únicos e ocorrências de itens de calendário recorrentes no intervalo especificado por **StartDate** e **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="121eb-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="121eb-136">Se o elemento **CalendarView** não for especificado em uma solicitação FindItem, o serviço Web retornará uma lista de itens de calendário únicos e itens de calendário mestre recorrentes.</span><span class="sxs-lookup"><span data-stu-id="121eb-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="121eb-137">As ocorrências de calendário de um item de calendário recorrente não são expandidas.</span><span class="sxs-lookup"><span data-stu-id="121eb-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="121eb-138">As consultas CalendarView devem usar apenas as propriedades a seguir, uma vez que oferecem suporte a consultas de calendário mais rápidas.</span><span class="sxs-lookup"><span data-stu-id="121eb-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="121eb-139">Propriedades do blob de recorrência</span><span class="sxs-lookup"><span data-stu-id="121eb-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="121eb-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="121eb-140">MapiStartTime</span></span>
    
- <span data-ttu-id="121eb-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="121eb-141">MapiEndTime</span></span>
    
- <span data-ttu-id="121eb-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="121eb-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="121eb-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="121eb-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="121eb-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="121eb-144">MapiSubject</span></span>
    
- <span data-ttu-id="121eb-145">Local</span><span class="sxs-lookup"><span data-stu-id="121eb-145">Location</span></span>
    
- <span data-ttu-id="121eb-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="121eb-146">AppointmentColor</span></span>
    
- <span data-ttu-id="121eb-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="121eb-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="121eb-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="121eb-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="121eb-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="121eb-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="121eb-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="121eb-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="121eb-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="121eb-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="121eb-152">Compromissostate</span><span class="sxs-lookup"><span data-stu-id="121eb-152">AppointmentState</span></span>
    
- <span data-ttu-id="121eb-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="121eb-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="121eb-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="121eb-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="121eb-155">Calculado a partir do blob de recorrência principal ou mestre</span><span class="sxs-lookup"><span data-stu-id="121eb-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="121eb-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="121eb-156">ItemId</span></span>
    
- <span data-ttu-id="121eb-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="121eb-157">IsRecurring</span></span>
    
- <span data-ttu-id="121eb-158">IsException</span><span class="sxs-lookup"><span data-stu-id="121eb-158">IsException</span></span>
    
- <span data-ttu-id="121eb-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="121eb-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="121eb-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="121eb-160">MapiStartTime</span></span>
    
- <span data-ttu-id="121eb-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="121eb-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="121eb-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="121eb-162">MapiEndTime</span></span>
    
- <span data-ttu-id="121eb-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="121eb-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="121eb-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="121eb-164">CalendarItemType</span></span>
    
- <span data-ttu-id="121eb-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="121eb-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="121eb-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="121eb-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="121eb-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="121eb-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="121eb-168">Propriedades do item do calendário mestre</span><span class="sxs-lookup"><span data-stu-id="121eb-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="121eb-169">EntryId</span><span class="sxs-lookup"><span data-stu-id="121eb-169">EntryId</span></span>
    
- <span data-ttu-id="121eb-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="121eb-170">ChangeKey</span></span>
    
- <span data-ttu-id="121eb-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="121eb-171">ItemClass</span></span>
    
- <span data-ttu-id="121eb-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="121eb-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="121eb-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="121eb-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="121eb-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="121eb-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="121eb-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="121eb-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="121eb-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="121eb-176">TimeZone</span></span>
    
- <span data-ttu-id="121eb-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="121eb-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="121eb-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="121eb-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="121eb-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="121eb-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="121eb-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="121eb-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="121eb-181">IsException</span><span class="sxs-lookup"><span data-stu-id="121eb-181">IsException</span></span>
    
- <span data-ttu-id="121eb-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="121eb-182">IsRecurring</span></span>
    
- <span data-ttu-id="121eb-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="121eb-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="121eb-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="121eb-184">ContainerClass</span></span>
    
- <span data-ttu-id="121eb-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="121eb-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="121eb-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="121eb-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="121eb-187">Categorias</span><span class="sxs-lookup"><span data-stu-id="121eb-187">Categories</span></span>
    
<span data-ttu-id="121eb-188">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="121eb-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="121eb-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="121eb-189">Example</span></span>

<span data-ttu-id="121eb-190">O exemplo a seguir mostra uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="121eb-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="121eb-191">Uma solicitação bem-sucedida retorna uma resposta que inclui itens de calendário iniciados em 2006-05-18T00:00:00-08:00 ou posterior e terminou antes de 2006-05-19T00:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="121eb-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="121eb-192">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="121eb-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="121eb-193">Namespace</span><span class="sxs-lookup"><span data-stu-id="121eb-193">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="121eb-194">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="121eb-194">Schema Name</span></span>  <br/> |<span data-ttu-id="121eb-195">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="121eb-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="121eb-196">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="121eb-196">Validation File</span></span>  <br/> |<span data-ttu-id="121eb-197">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="121eb-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="121eb-198">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="121eb-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="121eb-199">False</span><span class="sxs-lookup"><span data-stu-id="121eb-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="121eb-200">Confira também</span><span class="sxs-lookup"><span data-stu-id="121eb-200">See also</span></span>

- [<span data-ttu-id="121eb-201">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="121eb-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="121eb-202">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="121eb-202">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

