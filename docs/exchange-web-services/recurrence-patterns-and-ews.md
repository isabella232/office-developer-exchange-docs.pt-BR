---
title: Padrões de recorrência e EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Saiba mais sobre padrões de recorrência e séries recorrentes no Exchange.
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459325"
---
# <a name="recurrence-patterns-and-ews"></a><span data-ttu-id="0c8b3-103">Padrões de recorrência e EWS</span><span class="sxs-lookup"><span data-stu-id="0c8b3-103">Recurrence patterns and EWS</span></span>

<span data-ttu-id="0c8b3-104">Saiba mais sobre padrões de recorrência e séries recorrentes no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-104">Learn about recurrence patterns and recurring series in Exchange.</span></span>
  
<span data-ttu-id="0c8b3-105">Uma série recorrente é um compromisso ou uma reunião que se repete de acordo com um padrão definido.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-105">A recurring series is an appointment or meeting that repeats according to a defined pattern.</span></span> <span data-ttu-id="0c8b3-106">Uma série recorrente pode ter um número específico de ocorrências ou pode ser repetida indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-106">A recurring series can either have a specific number of occurrences or can repeat indefinitely.</span></span> <span data-ttu-id="0c8b3-107">Além disso, uma série recorrente pode ter exceções que não seguem o padrão do restante das ocorrências e podem ter ocorrências que foram excluídas do padrão.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-107">Additionally, a recurring series can have exceptions that don't follow the pattern of the rest of the occurrences, and can have occurrences that have been deleted from the pattern.</span></span> <span data-ttu-id="0c8b3-108">Você pode usar a API gerenciada do EWS e o EWS para trabalhar com séries recorrentes e seus itens de calendário associados.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-108">You can use the EWS Managed API and EWS to work with recurring series and their associated calendar items.</span></span>
  
## <a name="recurring-calendar-items"></a><span data-ttu-id="0c8b3-109">Itens de calendário recorrentes</span><span class="sxs-lookup"><span data-stu-id="0c8b3-109">Recurring calendar items</span></span>

<span data-ttu-id="0c8b3-110">Todos os itens de calendário se enquadram em uma das quatro categorias a seguir:</span><span class="sxs-lookup"><span data-stu-id="0c8b3-110">All calendar items fall into one of the following four categories:</span></span>
  
- <span data-ttu-id="0c8b3-111">Itens de calendário não recorrentes</span><span class="sxs-lookup"><span data-stu-id="0c8b3-111">Non-recurring calendar items</span></span>
    
- <span data-ttu-id="0c8b3-112">Mestres recorrentes</span><span class="sxs-lookup"><span data-stu-id="0c8b3-112">Recurring masters</span></span>
    
- <span data-ttu-id="0c8b3-113">Ocorrências em uma série</span><span class="sxs-lookup"><span data-stu-id="0c8b3-113">Occurrences in a series</span></span>
    
- <span data-ttu-id="0c8b3-114">Ocorrências modificadas em uma série, conhecidas como exceções</span><span class="sxs-lookup"><span data-stu-id="0c8b3-114">Modified occurrences in a series, known as exceptions</span></span>
    
<span data-ttu-id="0c8b3-115">Neste artigo, examinaremos os três tipos de itens de calendário que fazem parte de uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-115">In this article, we'll look at the three types of calendar items that are part of a recurring series.</span></span>
  
<span data-ttu-id="0c8b3-116">É útil entender como as séries recorrentes são implementadas no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-116">It's helpful to understand how recurring series are implemented on the Exchange server.</span></span> <span data-ttu-id="0c8b3-117">Em vez de criar um item distinto separado para cada ocorrência em uma série recorrente, o servidor cria apenas um item real no calendário, conhecido como mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-117">Instead of creating a separate distinct item for each occurrence in a recurring series, the server creates only one actual item in the calendar, known as the recurring master.</span></span> <span data-ttu-id="0c8b3-118">O formato de um mestre recorrente é muito semelhante a um compromisso não recorrente, com a adição de informações de padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-118">The format of a recurring master is very similar to a non-recurring appointment, with the addition of recurrence pattern information.</span></span> <span data-ttu-id="0c8b3-119">Em seguida, o servidor gera ocorrências com base no padrão de recorrência em resposta às solicitações de cliente para informações de compromisso, usando um processo chamado expansão.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-119">The server then generates occurrences based on the recurrence pattern in response to client requests for appointment information, using a process called expansion.</span></span> <span data-ttu-id="0c8b3-120">Essas ocorrências geradas não são permanentemente armazenadas no servidor.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-120">These generated occurrences are not permanently stored on the server.</span></span> <span data-ttu-id="0c8b3-121">Isso é importante entender, pois a forma como você pesquisa os itens de calendário determina quais informações você recebe e se a expansão ocorre.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-121">This is important to understand because the way that you search for calendar items determines what information you receive and whether expansion occurs.</span></span>
  
## <a name="recurrence-patterns"></a><span data-ttu-id="0c8b3-122">Padrões de recorrência</span><span class="sxs-lookup"><span data-stu-id="0c8b3-122">Recurrence patterns</span></span>

<span data-ttu-id="0c8b3-123">A parte principal de uma série recorrente que torna a expansão possível é o padrão de recorrência.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-123">The key piece to a recurring series that makes expansion possible is the recurrence pattern.</span></span> <span data-ttu-id="0c8b3-124">O padrão de recorrência é encontrado no mestre recorrente e descreve um conjunto de critérios para calcular as ocorrências com base na data e hora do mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-124">The recurrence pattern is found on the recurring master, and describes a set of criteria for calculating occurrences based on the date and time of the recurring master.</span></span>
  
<span data-ttu-id="0c8b3-125">**Tabela 1. Padrões de recorrência disponíveis**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-125">**Table 1. Available recurrence patterns**</span></span>

|<span data-ttu-id="0c8b3-126">**Classe de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-126">**EWS Managed API class**</span></span>|<span data-ttu-id="0c8b3-127">**Elemento do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-127">**EWS element**</span></span>|<span data-ttu-id="0c8b3-128">**Exemplos**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-128">**Examples**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="0c8b3-129">Recurrence. DailyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-129">Recurrence.DailyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-130">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-130">DailyRecurrence</span></span>](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-131">Repetir todos os dias.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-131">Repeat every day.</span></span>  <br/> <span data-ttu-id="0c8b3-132">Repetir a cada dia.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-132">Repeat every other day.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-133">Recurrence. MonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-133">Recurrence.MonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-134">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-134">AbsoluteMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-135">Repetir a cada mês no décimo dia do mês.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-135">Repeat every month on the tenth day of the month.</span></span>  <br/> <span data-ttu-id="0c8b3-136">Repetir a cada mês no primeiro dia do mês.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-136">Repeat every other month on the twenty-first day of the month.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-137">Recurrence. RelativeMonthlyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-137">Recurrence.RelativeMonthlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-138">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-138">RelativeMonthlyRecurrence</span></span>](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-139">Repita a segunda terça-feira de cada mês.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-139">Repeat on the second Tuesday of every month.</span></span>  <br/> <span data-ttu-id="0c8b3-140">Repita a terceira quinta-feira do mês a cada três meses.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-140">Repeat on the third Thursday of the month every three months.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-141">Recurrence. RelativeYearlyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-141">Recurrence.RelativeYearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-142">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-142">RelativeYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-143">Repita na primeira segunda-feira de agosto a cada ano.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-143">Repeat on the first Monday of August every year.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-144">Recurrence. WeeklyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-144">Recurrence.WeeklyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-145">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-145">WeeklyRecurrence</span></span>](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-146">Repetir a cada segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-146">Repeat every Monday.</span></span>  <br/> <span data-ttu-id="0c8b3-147">Repita todas as terças e quinta-feira a cada semana.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-147">Repeat every Tuesday and Thursday every other week.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-148">Recurrence. YearlyPattern</span><span class="sxs-lookup"><span data-stu-id="0c8b3-148">Recurrence.YearlyPattern</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-149">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-149">AbsoluteYearlyRecurrence</span></span>](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-150">Repita no dia 1º de setembro a cada ano.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-150">Repeat on September 1st every year.</span></span>  <br/> |
   
<span data-ttu-id="0c8b3-151">A outra informação importante para um padrão de recorrência é quando a recorrência termina.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-151">The other important piece of information for a recurrence pattern is when the recurrence ends.</span></span> <span data-ttu-id="0c8b3-152">Isso pode ser expresso como um número definido de ocorrências, como uma data final ou como sem final.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-152">This can be expressed as either a set number of occurrences, as an end date, or as having no end.</span></span>
  
<span data-ttu-id="0c8b3-153">**Tabela 2. Opções para o final de uma série recorrente**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-153">**Table 2. Options for the end of a recurring series**</span></span>

|<span data-ttu-id="0c8b3-154">**Método/propriedade da API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-154">**EWS Managed API method/property**</span></span>|<span data-ttu-id="0c8b3-155">**Elemento do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-155">**EWS element**</span></span>|<span data-ttu-id="0c8b3-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-156">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="0c8b3-157">Recurrence. NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="0c8b3-157">Recurrence.NumberOfOccurrences</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-158">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-158">NumberedRecurrence</span></span>](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-159">O valor dessa propriedade ou elemento Especifica o número de ocorrências.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-159">The value of this property or element specifies the number of occurrences.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-160">Recurrence. EndDate</span><span class="sxs-lookup"><span data-stu-id="0c8b3-160">Recurrence.EndDate</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-161">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-161">EndDateRecurrence</span></span>](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-162">A última ocorrência na série cai ou antes da data especificada por essa propriedade ou elemento.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-162">The last occurrence in the series falls on or before the date specified by this property or element.</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-163">Recurrence. HasEnd</span><span class="sxs-lookup"><span data-stu-id="0c8b3-163">Recurrence.HasEnd</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="0c8b3-164">Recurrence. NeverEnds</span><span class="sxs-lookup"><span data-stu-id="0c8b3-164">Recurrence.NeverEnds</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="0c8b3-165">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="0c8b3-165">NoEndRecurrence</span></span>](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |<span data-ttu-id="0c8b3-166">A série não tem fim.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-166">The series has no end.</span></span>  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a><span data-ttu-id="0c8b3-167">Exibições expandidas vs. não expandidas</span><span class="sxs-lookup"><span data-stu-id="0c8b3-167">Expanded vs. non-expanded views</span></span>

<span data-ttu-id="0c8b3-168">O uso do método **FindAppointments** na API gerenciada do EWS (ou na operação **FindItem** com um elemento **CalendarView** no EWS) invoca o processo de expansão.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-168">Using the **FindAppointments** method in the EWS Managed API (or the **FindItem** operation with a **CalendarView** element in EWS) invokes the expansion process.</span></span> <span data-ttu-id="0c8b3-169">Isso oculta compromissos mestre recorrentes do conjunto de resultados e, em vez disso, apresenta uma visão expandida dessa série recorrente.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-169">This hides recurring master appointments from the result set, and instead presents an expanded view of that recurring series.</span></span> <span data-ttu-id="0c8b3-170">As ocorrências de e exceções para o mestre recorrente que estão dentro dos parâmetros do modo de exibição de calendário são incluídas no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-170">Occurrences of and exceptions to the recurring master that fall within the parameters of the calendar view are included in the result set.</span></span> <span data-ttu-id="0c8b3-171">Por outro lado, usar o método **FindItems** na API gerenciada do EWS (ou na operação **FindItem** com um elemento **IndexedPageItemView** ou **FractionalPageItemView** no EWS), não invoca o processo de expansão, e as ocorrências e exceções não estão incluídas.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-171">Conversely, using the **FindItems** method in the EWS Managed API (or the **FindItem** operation with a **IndexedPageItemView** or **FractionalPageItemView** element in EWS), does not invoke the expansion process, and occurrences and exceptions are not included.</span></span> <span data-ttu-id="0c8b3-172">Vejamos um exemplo que compara os dois métodos.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-172">Let's look at an example comparing the two methods.</span></span> 
  
<span data-ttu-id="0c8b3-173">**Tabela 3. Métodos e operações para localizar compromissos**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-173">**Table 3. Methods and operations for finding appointments**</span></span>

|<span data-ttu-id="0c8b3-174">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-174">**EWS Managed API method**</span></span>|<span data-ttu-id="0c8b3-175">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-175">**EWS operation**</span></span>|<span data-ttu-id="0c8b3-176">**Expande a série?**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-176">**Expands series?**</span></span>|<span data-ttu-id="0c8b3-177">**Itens incluídos nos resultados**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-177">**Items included in results**</span></span>|
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="0c8b3-178">ExchangeService. FindAppointments</span><span class="sxs-lookup"><span data-stu-id="0c8b3-178">ExchangeService.FindAppointments</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="0c8b3-179">[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0c8b3-179">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="0c8b3-180">Sim</span><span class="sxs-lookup"><span data-stu-id="0c8b3-180">Yes</span></span>  <br/> |<span data-ttu-id="0c8b3-181">Compromissos não recorrentes, ocorrências únicas de séries recorrentes e exceções à série recorrente</span><span class="sxs-lookup"><span data-stu-id="0c8b3-181">Non-recurring appointments, single occurrences of recurring series, and exceptions to recurring series</span></span>  <br/> |
|[<span data-ttu-id="0c8b3-182">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="0c8b3-182">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="0c8b3-183">[Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou um elemento [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0c8b3-183">[FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="0c8b3-184">Não</span><span class="sxs-lookup"><span data-stu-id="0c8b3-184">No</span></span>  <br/> |<span data-ttu-id="0c8b3-185">Compromissos não recorrentes e compromissos mestre recorrentes</span><span class="sxs-lookup"><span data-stu-id="0c8b3-185">Non-recurring appointments and recurring master appointments</span></span>  <br/> |
   
<span data-ttu-id="0c8b3-186">Sadie acabou de assinar seu filho para a equipe de nada.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-186">Sadie has just signed her son up for swim team.</span></span> <span data-ttu-id="0c8b3-187">A equipe tem a prática toda quarta-feira de manhã às 8:30 AM, a partir de 2 de julho, com a última sessão em 6 de agosto.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-187">The team has practice every Wednesday morning at 8:30 AM, starting July 2, with the last practice being on August 6.</span></span> <span data-ttu-id="0c8b3-188">Não quer esquecer da prática, o Sadie adiciona um compromisso recorrente ao seu calendário para lembrá-lo.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-188">Not wanting to forget about practice, Sadie adds a recurring appointment to her calendar to remind her.</span></span>
  
<span data-ttu-id="0c8b3-189">**Tabela 4. Compromisso recorrente do Sadie**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-189">**Table 4. Sadie's recurring appointment**</span></span>

|<span data-ttu-id="0c8b3-190">**Campo de compromisso**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-190">**Appointment field**</span></span>|<span data-ttu-id="0c8b3-191">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0c8b3-191">**Value**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c8b3-192">Assunto</span><span class="sxs-lookup"><span data-stu-id="0c8b3-192">Subject</span></span>  <br/> |<span data-ttu-id="0c8b3-193">Prática de equipe de nada</span><span class="sxs-lookup"><span data-stu-id="0c8b3-193">Swim Team Practice</span></span>  <br/> |
|<span data-ttu-id="0c8b3-194">Início</span><span class="sxs-lookup"><span data-stu-id="0c8b3-194">Start</span></span>  <br/> |<span data-ttu-id="0c8b3-195">2 de julho de 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="0c8b3-195">July 2, 2014 8:30 AM</span></span>  <br/> |
|<span data-ttu-id="0c8b3-196">Final</span><span class="sxs-lookup"><span data-stu-id="0c8b3-196">End</span></span>  <br/> |<span data-ttu-id="0c8b3-197">2 de julho de 2014 10:00 AM</span><span class="sxs-lookup"><span data-stu-id="0c8b3-197">July 2, 2014 10:00 AM</span></span>  <br/> |
|<span data-ttu-id="0c8b3-198">Reaparecer</span><span class="sxs-lookup"><span data-stu-id="0c8b3-198">Recurs</span></span>  <br/> |<span data-ttu-id="0c8b3-199">Toda quarta-feira</span><span class="sxs-lookup"><span data-stu-id="0c8b3-199">Every Wednesday</span></span>  <br/> |
|<span data-ttu-id="0c8b3-200">Última ocorrência</span><span class="sxs-lookup"><span data-stu-id="0c8b3-200">Last occurrence</span></span>  <br/> |<span data-ttu-id="0c8b3-201">6 de agosto de 2014 8:30 AM</span><span class="sxs-lookup"><span data-stu-id="0c8b3-201">August 6, 2014 8:30 AM</span></span>  <br/> |
   
<span data-ttu-id="0c8b3-202">Uma visão rápida de um calendário mostra que a equipe terá um total de seis práticas.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-202">A quick look at a calendar shows that the team will have a total of six practices.</span></span> <span data-ttu-id="0c8b3-203">No entanto, não há seis itens de compromisso distintos no calendário.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-203">However, there aren't six distinct appointment items in the calendar.</span></span> <span data-ttu-id="0c8b3-204">Em vez disso, há apenas um compromisso mestre recorrente que representa a série.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-204">Instead, there is just one recurring master appointment representing the series.</span></span>
  
<span data-ttu-id="0c8b3-205">Agora, vamos examinar a localização de compromissos no calendário do Sadie que ocorrem no mês de julho.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-205">Now let's look at finding appointments on Sadie's calendar that occur within the month of July.</span></span> <span data-ttu-id="0c8b3-206">O exemplo de código a seguir usa o método **FindItems** na API gerenciada do Exchange para produzir uma visão não expandida do calendário de Sadie.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-206">The following code example uses the **FindItems** method in the Exchange Managed API to produce a non-expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="0c8b3-207">Esse código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0c8b3-207">That code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with an [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0c8b3-208">A resposta do servidor inclui apenas um único item, o mestre recorrente, indicado pelo valor do elemento [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de **RecurringMaster**.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-208">The server's response includes only a single item, the recurring master, indicated by the [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element value of **RecurringMaster**.</span></span> <span data-ttu-id="0c8b3-209">O valor do elemento [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-209">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c8b3-210">Agora, vamos comparar com um modo de exibição expandido.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-210">Now let's compare with an expanded view.</span></span> <span data-ttu-id="0c8b3-211">O exemplo de código a seguir usa o método **FindAppointments** na API gerenciada do EWS para criar uma exibição expandida do calendário de Sadie.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-211">The following code example uses the **FindAppointments** method in the EWS Managed API to create an expanded view of Sadie's calendar.</span></span> 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

<span data-ttu-id="0c8b3-212">Esse código resulta na seguinte solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com um elemento [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0c8b3-212">This code results in the following [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request with a [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0c8b3-213">Desta vez, a resposta do servidor inclui cinco ocorrências, uma para cada quarta-feira em julho.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-213">This time, the server response includes five occurrences, one for each Wednesday in July.</span></span> <span data-ttu-id="0c8b3-214">Os elementos [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) desses itens têm um valor de **ocorrência**.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-214">The [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) elements on these items all have a value of **Occurrence**.</span></span> <span data-ttu-id="0c8b3-215">Observe que o mestre recorrente não está presente na resposta.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-215">Note that the recurring master is not present in the response.</span></span> <span data-ttu-id="0c8b3-216">Os valores dos elementos [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-216">The values of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="0c8b3-217">Após ter um mestre recorrente, uma ocorrência ou uma exceção, você sempre poderá [recuperar os outros itens relacionados](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0c8b3-217">After you have a recurring master, an occurrence, or an exception, you can always [retrieve the other related items](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="0c8b3-218">Devido a uma ocorrência ou exceção, você pode recuperar o mestre recorrente e vice-versa.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-218">Given an occurrence or exception, you can retrieve the recurring master, and vice versa.</span></span>
  
## <a name="working-with-recurring-calendar-items"></a><span data-ttu-id="0c8b3-219">Trabalhar com itens de calendário recorrentes</span><span class="sxs-lookup"><span data-stu-id="0c8b3-219">Working with recurring calendar items</span></span>

<span data-ttu-id="0c8b3-220">Você usa todos os mesmos métodos e operações para trabalhar com a série recorrente ao usar o para trabalhar com itens de calendário não recorrentes.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-220">You use all the same methods and operations to work with recurring series as you use to work with non-recurring calendar items.</span></span> <span data-ttu-id="0c8b3-221">A diferença é que, dependendo do item que você usa para invocar esses métodos ou operações, as ações que você executa podem ser aplicadas à série inteira ou apenas a uma única ocorrência.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-221">The difference is that, depending on the item you use to invoke those methods or operations, the actions you take can apply to the entire series, or just a single occurrence.</span></span> <span data-ttu-id="0c8b3-222">[As ações realizadas no mestre recorrente](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) se aplicarão a todas as ocorrências da série, enquanto as [ações realizadas para uma única ocorrência ou exceção](how-to-update-a-recurring-series-by-using-ews.md) só serão aplicadas a essa ocorrência ou exceção.</span><span class="sxs-lookup"><span data-stu-id="0c8b3-222">[Actions taken on the recurring master](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) will apply to all occurrences in the series, while [actions taken to a single occurrence or exception](how-to-update-a-recurring-series-by-using-ews.md) will only apply to that occurrence or exception.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="0c8b3-223">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="0c8b3-223">In this section</span></span>

- [<span data-ttu-id="0c8b3-224">Acessar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-224">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0c8b3-225">Criar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-225">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0c8b3-226">Excluir compromissos em uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-226">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="0c8b3-227">Atualizar uma série recorrente usando o EWS</span><span class="sxs-lookup"><span data-stu-id="0c8b3-227">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="0c8b3-228">Atualizar uma série recorrente usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-228">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="0c8b3-229">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0c8b3-229">See also</span></span>


- [<span data-ttu-id="0c8b3-230">Calendários e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-230">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="0c8b3-231">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-231">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="0c8b3-232">Obter compromissos e reuniões usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0c8b3-232">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

