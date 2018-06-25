---
title: Operação UpdateItem (tarefa)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: A operação UpdateItem é usada para atualizar as propriedades de item de tarefa no armazenamento do Exchange.
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837912"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="f0333-103">Operação UpdateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="f0333-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="f0333-104">A operação UpdateItem é usada para atualizar as propriedades de item de tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0333-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0333-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="f0333-105">Remarks</span></span>

<span data-ttu-id="f0333-106">Você não pode usar os serviços Web do Exchange para enviar solicitações de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f0333-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="f0333-107">Serviços Web do Exchange pode retornar as solicitações de tarefa que são criadas por MicrosoftOfficeOutlook.</span><span class="sxs-lookup"><span data-stu-id="f0333-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="f0333-108">Se já tiver sido enviada a uma solicitação de tarefa, uma solicitação para atualizar a tarefa retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="f0333-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="f0333-109">Atualizando a ocorrência atual de uma tarefa recorrente</span><span class="sxs-lookup"><span data-stu-id="f0333-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="f0333-110">O resultado de uma operação de UpdateItem em tarefas recorrentes difere do resultado da operação UpdateItem sobre uma tarefa única e nonrecurring.</span><span class="sxs-lookup"><span data-stu-id="f0333-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="f0333-111">Alterações em uma ocorrência de uma tarefa recorrente causar únicas tarefas a serem gerados quando as seguintes atualizações são feitas:</span><span class="sxs-lookup"><span data-stu-id="f0333-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="f0333-112">A propriedade do status de uma tarefa recorrente regeneração ou nonregenerating é definida como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="f0333-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="f0333-113">A data de início ou data de término de uma tarefa recorrente nonregenerating é alterada.</span><span class="sxs-lookup"><span data-stu-id="f0333-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="f0333-114">Por exemplo, se uma solicitação de **UpdateItem** define o valor de concluído de uma tarefa recorrente como **true**, o **UpdateItemResponse** incluirá uma nova Id e ChangeKey que representam uma tarefa único recém-criado.</span><span class="sxs-lookup"><span data-stu-id="f0333-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="f0333-115">A Id que foi incluída na solicitação ainda é válida e a tarefa recorrente que é representada por esse Id foi atualizada para representar a próxima ocorrência.</span><span class="sxs-lookup"><span data-stu-id="f0333-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="f0333-116">O que foi incluída na solicitação ChangeKey não é mais válido porque a tarefa recorrente foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="f0333-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="f0333-117">Você pode usar a [operação GetItem](getitem-operation.md) para obter as últimas **ChangeKey** para a tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="f0333-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="f0333-118">Para tarefas nonrecurring ou a última ocorrência de uma tarefa recorrente, a resposta UpdateItem retorna a mesma **Id** que foi passado para ele e retorna que o associado atualizado **ChangeKey**.</span><span class="sxs-lookup"><span data-stu-id="f0333-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f0333-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="f0333-119">See also</span></span>



[<span data-ttu-id="f0333-120">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="f0333-120">UpdateItem operation</span></span>](updateitem-operation.md)

