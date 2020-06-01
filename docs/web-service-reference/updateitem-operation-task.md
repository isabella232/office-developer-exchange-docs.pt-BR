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
description: A operação UpdateItem é usada para atualizar as propriedades do item de tarefa no repositório do Exchange.
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459802"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="a068a-103">Operação UpdateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="a068a-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="a068a-104">A operação UpdateItem é usada para atualizar as propriedades do item de tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a068a-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a068a-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="a068a-105">Remarks</span></span>

<span data-ttu-id="a068a-106">Você não pode usar os serviços Web do Exchange para enviar solicitações de tarefa.</span><span class="sxs-lookup"><span data-stu-id="a068a-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="a068a-107">Os serviços Web do Exchange podem retornar solicitações de tarefas criadas pelo MicrosoftOfficeOutlook.</span><span class="sxs-lookup"><span data-stu-id="a068a-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="a068a-108">Se uma solicitação de tarefa já tiver sido enviada, uma solicitação para atualizar a tarefa retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="a068a-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="a068a-109">Atualizando a ocorrência atual de uma tarefa recorrente</span><span class="sxs-lookup"><span data-stu-id="a068a-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="a068a-110">O resultado de uma operação UpdateItem em tarefas recorrentes difere do resultado da operação UpdateItem em uma única tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a068a-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="a068a-111">Alterações a uma ocorrência de uma tarefa recorrente fazem com que as tarefas individuais sejam geradas quando as seguintes atualizações são feitas:</span><span class="sxs-lookup"><span data-stu-id="a068a-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="a068a-112">A propriedade status de uma tarefa regeradora ou nonregenerating recorrente está definida como **concluída**.</span><span class="sxs-lookup"><span data-stu-id="a068a-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="a068a-113">A data de início ou a data de término de uma tarefa recorrente de nonregenerating é alterada.</span><span class="sxs-lookup"><span data-stu-id="a068a-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="a068a-114">Por exemplo, se uma solicitação **UpdateItem** define o valor concluído de uma tarefa recorrente como **true**, o **UpdateItemResponse** incluirá uma nova ID e ChangeKey que representam uma tarefa única recém-criada.</span><span class="sxs-lookup"><span data-stu-id="a068a-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="a068a-115">A ID que foi incluída na solicitação ainda é válida e a tarefa recorrente representada pela ID foi atualizada para representar a próxima ocorrência.</span><span class="sxs-lookup"><span data-stu-id="a068a-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="a068a-116">O ChangeKey que foi incluído na solicitação não é mais válido porque a tarefa recorrente foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="a068a-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="a068a-117">Você pode usar a [operação GetItem](getitem-operation.md) para obter o **ChangeKey** mais recente para a tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a068a-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="a068a-118">Para tarefas recorrentes ou para a última ocorrência de uma tarefa recorrente, a resposta UpdateItem retorna a mesma **ID** que foi passada e retorna a **ChangeKey**atualizada associada.</span><span class="sxs-lookup"><span data-stu-id="a068a-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a068a-119">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a068a-119">See also</span></span>



[<span data-ttu-id="a068a-120">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a068a-120">UpdateItem operation</span></span>](updateitem-operation.md)

