---
title: Exibição de calendário
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
description: O elemento CalendarView define uma operação FindItem como retornar itens de calendário em um conjunto que aparecem em um calendário.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751369"
---
# <a name="calendarview"></a><span data-ttu-id="6fb90-103">Exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="6fb90-103">CalendarView</span></span>

<span data-ttu-id="6fb90-104">O elemento **CalendarView** define uma [operação FindItem](finditem-operation.md) como retornar itens de calendário em um conjunto que aparecem em um calendário.</span><span class="sxs-lookup"><span data-stu-id="6fb90-104">The **CalendarView** element defines a [FindItem operation](finditem-operation.md) as returning calendar items in a set as they appear in a calendar.</span></span> 
  
[<span data-ttu-id="6fb90-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="6fb90-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="6fb90-106">Exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="6fb90-106">CalendarView</span></span>](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

<span data-ttu-id="6fb90-107">**Exibição de calendário**</span><span class="sxs-lookup"><span data-stu-id="6fb90-107">**CalendarView**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6fb90-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6fb90-108">Attributes and elements</span></span>

<span data-ttu-id="6fb90-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6fb90-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fb90-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6fb90-110">Attributes</span></span>

|<span data-ttu-id="6fb90-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="6fb90-111">**Attribute**</span></span>|<span data-ttu-id="6fb90-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fb90-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fb90-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="6fb90-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="6fb90-114">Descreve o número máximo de resultados a serem retornados na resposta FindItem.</span><span class="sxs-lookup"><span data-stu-id="6fb90-114">Describes the maximum number of results to return in the FindItem response.</span></span>  <br/> |
|<span data-ttu-id="6fb90-115">**StartDate**</span><span class="sxs-lookup"><span data-stu-id="6fb90-115">**StartDate**</span></span> <br/> |<span data-ttu-id="6fb90-116">Identifica o início de um período de tempo consultado para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="6fb90-116">Identifies the start of a time span queried for calendar items.</span></span> <span data-ttu-id="6fb90-117">Todos os itens de calendário que têm uma hora de término que seja antes **StartDate** não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="6fb90-117">All calendar items that have an end time that is before **StartDate** will not be returned.</span></span> <span data-ttu-id="6fb90-118">O valor da **StartDate** pode ser especificado no formato tempo universal coordenado (UTC), como de 2006-01-02T12:00:00Z, ou em um formato que o deslocamento de hora local e fuso horário estiver especificado, como 2006-01-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="6fb90-118">The value of **StartDate** can be specified in coordinated universal time (UTC) format, as in 2006-01-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-01-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="6fb90-119">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6fb90-119">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6fb90-120">**EndDate**</span><span class="sxs-lookup"><span data-stu-id="6fb90-120">**EndDate**</span></span> <br/> |<span data-ttu-id="6fb90-121">Identifica o final de um período de tempo consultado para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="6fb90-121">Identifies the end of a time span queried for calendar items.</span></span> <span data-ttu-id="6fb90-122">Todos os itens de calendário que têm uma hora de início em ou após **EndDate** não serão retornados.</span><span class="sxs-lookup"><span data-stu-id="6fb90-122">All calendar items that have a start time that is on or after **EndDate** will not be returned.</span></span> <span data-ttu-id="6fb90-123">O valor da **EndDate** pode ser especificado no formato UTC, como de 2006-02-02T12:00:00Z, ou em um formato que o deslocamento de hora local e fuso horário estiver especificado, como 2006-02-02T04:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="6fb90-123">The value of **EndDate** can be specified in UTC format, as in 2006-02-02T12:00:00Z, or in a format where local time and time zone offset is specified, as in 2006-02-02T04:00:00-08:00.</span></span>  <br/><br/><span data-ttu-id="6fb90-124">**EndDate** deve ser maior ou igual a **StartDate**; Caso contrário, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="6fb90-124">**EndDate** must be greater than or equal to **StartDate**; otherwise an error is returned.</span></span> <span data-ttu-id="6fb90-125">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6fb90-125">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6fb90-126">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6fb90-126">Child elements</span></span>

<span data-ttu-id="6fb90-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6fb90-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6fb90-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6fb90-128">Parent elements</span></span>

|<span data-ttu-id="6fb90-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fb90-129">**Element**</span></span>|<span data-ttu-id="6fb90-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fb90-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fb90-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="6fb90-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="6fb90-132">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6fb90-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="6fb90-133">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6fb90-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fb90-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fb90-134">Remarks</span></span>

<span data-ttu-id="6fb90-135">Se o elemento de **exibição de calendário** for especificado em uma solicitação de FindItem, o serviço Web retorna uma lista de itens de calendário único e ocorrências de itens de calendário recorrentes dentro do intervalo especificado pelo **StartDate** e **EndDate**.</span><span class="sxs-lookup"><span data-stu-id="6fb90-135">If the **CalendarView** element is specified in a FindItem request, the Web service returns a list of single calendar items and occurrences of recurring calendar items within the range specified by **StartDate** and **EndDate**.</span></span>
  
<span data-ttu-id="6fb90-136">Se o elemento de **exibição de calendário** não for especificado em uma solicitação de FindItem, o serviço Web retorna uma lista de itens de calendário único e itens de calendário mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="6fb90-136">If the **CalendarView** element is not specified in a FindItem request, the Web service returns a list of single calendar items and recurring master calendar items.</span></span> <span data-ttu-id="6fb90-137">Ocorrências de calendário de um item de calendário recorrente não são expandidas.</span><span class="sxs-lookup"><span data-stu-id="6fb90-137">Calendar occurrences of a recurring calendar item are not expanded.</span></span> 
  
<span data-ttu-id="6fb90-138">Consultas CalendarView só devem fazer use das propriedades a seguir, desde que eles oferecem suporte a consultas de calendário mais rápidas.</span><span class="sxs-lookup"><span data-stu-id="6fb90-138">CalendarView queries should only make use of the following properties since they support faster calendar queries.</span></span>
  
### <a name="recurrence-blob-properties"></a><span data-ttu-id="6fb90-139">Propriedades de blob de recorrência</span><span class="sxs-lookup"><span data-stu-id="6fb90-139">Recurrence blob properties</span></span>
  
- <span data-ttu-id="6fb90-140">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="6fb90-140">MapiStartTime</span></span>
    
- <span data-ttu-id="6fb90-141">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="6fb90-141">MapiEndTime</span></span>
    
- <span data-ttu-id="6fb90-142">SubjectPrefixInternal</span><span class="sxs-lookup"><span data-stu-id="6fb90-142">SubjectPrefixInternal</span></span>
    
- <span data-ttu-id="6fb90-143">NormalizedSubjectInternal</span><span class="sxs-lookup"><span data-stu-id="6fb90-143">NormalizedSubjectInternal</span></span>
    
- <span data-ttu-id="6fb90-144">MapiSubject</span><span class="sxs-lookup"><span data-stu-id="6fb90-144">MapiSubject</span></span>
    
- <span data-ttu-id="6fb90-145">Local</span><span class="sxs-lookup"><span data-stu-id="6fb90-145">Location</span></span>
    
- <span data-ttu-id="6fb90-146">AppointmentColor</span><span class="sxs-lookup"><span data-stu-id="6fb90-146">AppointmentColor</span></span>
    
- <span data-ttu-id="6fb90-147">MapiIsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="6fb90-147">MapiIsAllDayEvent</span></span>
    
- <span data-ttu-id="6fb90-148">MapiHasAttachment</span><span class="sxs-lookup"><span data-stu-id="6fb90-148">MapiHasAttachment</span></span>
    
- <span data-ttu-id="6fb90-149">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="6fb90-149">FreeBusyStatus</span></span>
    
- <span data-ttu-id="6fb90-150">ReminderIsSetInternal</span><span class="sxs-lookup"><span data-stu-id="6fb90-150">ReminderIsSetInternal</span></span>
    
- <span data-ttu-id="6fb90-151">ReminderMinutesBeforeStartInternal</span><span class="sxs-lookup"><span data-stu-id="6fb90-151">ReminderMinutesBeforeStartInternal</span></span>
    
- <span data-ttu-id="6fb90-152">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="6fb90-152">AppointmentState</span></span>
    
- <span data-ttu-id="6fb90-153">AllAttachmentsHidden</span><span class="sxs-lookup"><span data-stu-id="6fb90-153">AllAttachmentsHidden</span></span>
    
- <span data-ttu-id="6fb90-154">ChangeHighlight</span><span class="sxs-lookup"><span data-stu-id="6fb90-154">ChangeHighlight</span></span>
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a><span data-ttu-id="6fb90-155">Calculado a partir do blob de recorrência principal ou do mestre</span><span class="sxs-lookup"><span data-stu-id="6fb90-155">Calculated from the primary recurrence blob or master</span></span>
  
- <span data-ttu-id="6fb90-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="6fb90-156">ItemId</span></span>
    
- <span data-ttu-id="6fb90-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="6fb90-157">IsRecurring</span></span>
    
- <span data-ttu-id="6fb90-158">IsException</span><span class="sxs-lookup"><span data-stu-id="6fb90-158">IsException</span></span>
    
- <span data-ttu-id="6fb90-159">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="6fb90-159">AppointmentRecurring</span></span>
    
- <span data-ttu-id="6fb90-160">MapiStartTime</span><span class="sxs-lookup"><span data-stu-id="6fb90-160">MapiStartTime</span></span>
    
- <span data-ttu-id="6fb90-161">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="6fb90-161">MapiPRStartDate</span></span>
    
- <span data-ttu-id="6fb90-162">MapiEndTime</span><span class="sxs-lookup"><span data-stu-id="6fb90-162">MapiEndTime</span></span>
    
- <span data-ttu-id="6fb90-163">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="6fb90-163">MapiPREndDate</span></span>
    
- <span data-ttu-id="6fb90-164">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="6fb90-164">CalendarItemType</span></span>
    
- <span data-ttu-id="6fb90-165">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="6fb90-165">GlobalObjectId</span></span>
    
- <span data-ttu-id="6fb90-166">TimeZoneDefinitionStart</span><span class="sxs-lookup"><span data-stu-id="6fb90-166">TimeZoneDefinitionStart</span></span>
    
- <span data-ttu-id="6fb90-167">TimeZoneDefinitionEnd</span><span class="sxs-lookup"><span data-stu-id="6fb90-167">TimeZoneDefinitionEnd</span></span>
    
### <a name="master-calendar-item-properties"></a><span data-ttu-id="6fb90-168">Propriedades de item de calendário mestre</span><span class="sxs-lookup"><span data-stu-id="6fb90-168">Master calendar item properties</span></span>
  
- <span data-ttu-id="6fb90-169">EntryId</span><span class="sxs-lookup"><span data-stu-id="6fb90-169">EntryId</span></span>
    
- <span data-ttu-id="6fb90-170">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6fb90-170">ChangeKey</span></span>
    
- <span data-ttu-id="6fb90-171">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6fb90-171">ItemClass</span></span>
    
- <span data-ttu-id="6fb90-172">SentRepresentingEmailAddress</span><span class="sxs-lookup"><span data-stu-id="6fb90-172">SentRepresentingEmailAddress</span></span>
    
- <span data-ttu-id="6fb90-173">SentRepresentingDisplayName</span><span class="sxs-lookup"><span data-stu-id="6fb90-173">SentRepresentingDisplayName</span></span>
    
- <span data-ttu-id="6fb90-174">SentRepresentingEntryId</span><span class="sxs-lookup"><span data-stu-id="6fb90-174">SentRepresentingEntryId</span></span>
    
- <span data-ttu-id="6fb90-175">AppointmentRecurrenceBlob</span><span class="sxs-lookup"><span data-stu-id="6fb90-175">AppointmentRecurrenceBlob</span></span>
    
- <span data-ttu-id="6fb90-176">TimeZone</span><span class="sxs-lookup"><span data-stu-id="6fb90-176">TimeZone</span></span>
    
- <span data-ttu-id="6fb90-177">TimeZoneBlob</span><span class="sxs-lookup"><span data-stu-id="6fb90-177">TimeZoneBlob</span></span>
    
- <span data-ttu-id="6fb90-178">TimeZoneDefinitionRecurring</span><span class="sxs-lookup"><span data-stu-id="6fb90-178">TimeZoneDefinitionRecurring</span></span>
    
- <span data-ttu-id="6fb90-179">CleanGlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="6fb90-179">CleanGlobalObjectId</span></span>
    
- <span data-ttu-id="6fb90-180">AppointmentRecurring</span><span class="sxs-lookup"><span data-stu-id="6fb90-180">AppointmentRecurring</span></span>
    
- <span data-ttu-id="6fb90-181">IsException</span><span class="sxs-lookup"><span data-stu-id="6fb90-181">IsException</span></span>
    
- <span data-ttu-id="6fb90-182">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="6fb90-182">IsRecurring</span></span>
    
- <span data-ttu-id="6fb90-183">MapiSensitivity</span><span class="sxs-lookup"><span data-stu-id="6fb90-183">MapiSensitivity</span></span>
    
- <span data-ttu-id="6fb90-184">ContainerClass</span><span class="sxs-lookup"><span data-stu-id="6fb90-184">ContainerClass</span></span>
    
- <span data-ttu-id="6fb90-185">MapiPRStartDate</span><span class="sxs-lookup"><span data-stu-id="6fb90-185">MapiPRStartDate</span></span>
    
- <span data-ttu-id="6fb90-186">MapiPREndDate</span><span class="sxs-lookup"><span data-stu-id="6fb90-186">MapiPREndDate</span></span>
    
- <span data-ttu-id="6fb90-187">Categories</span><span class="sxs-lookup"><span data-stu-id="6fb90-187">Categories</span></span>
    
<span data-ttu-id="6fb90-188">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6fb90-188">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="6fb90-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fb90-189">Example</span></span>

<span data-ttu-id="6fb90-190">O exemplo a seguir mostra uma solicitação FindItem.</span><span class="sxs-lookup"><span data-stu-id="6fb90-190">The following example shows a FindItem request.</span></span> <span data-ttu-id="6fb90-191">Uma solicitação bem-sucedida retornará uma resposta que inclui itens de calendário iniciados de 2006-05-18T00:00:00-08:00 ou depois e finalizada antes de 2006-05-19T00:00:00-08:00.</span><span class="sxs-lookup"><span data-stu-id="6fb90-191">A successful request returns a response that includes calendar items that started at 2006-05-18T00:00:00-08:00 or after and ended before 2006-05-19T00:00:00-08:00.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="6fb90-192">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6fb90-192">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fb90-193">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fb90-193">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6fb90-194">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6fb90-194">Schema Name</span></span>  <br/> |<span data-ttu-id="6fb90-195">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6fb90-195">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6fb90-196">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6fb90-196">Validation File</span></span>  <br/> |<span data-ttu-id="6fb90-197">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6fb90-197">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6fb90-198">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6fb90-198">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fb90-199">False</span><span class="sxs-lookup"><span data-stu-id="6fb90-199">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fb90-200">Ver também</span><span class="sxs-lookup"><span data-stu-id="6fb90-200">See also</span></span>

- [<span data-ttu-id="6fb90-201">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="6fb90-201">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="6fb90-202">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="6fb90-202">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

