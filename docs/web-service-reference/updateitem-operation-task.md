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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459802"
---
# <a name="updateitem-operation-task"></a>Operação UpdateItem (tarefa)

A operação UpdateItem é usada para atualizar as propriedades do item de tarefa no repositório do Exchange.
  
## <a name="remarks"></a>Comentários

Você não pode usar os serviços Web do Exchange para enviar solicitações de tarefa. Os serviços Web do Exchange podem retornar solicitações de tarefas criadas pelo MicrosoftOfficeOutlook. Se uma solicitação de tarefa já tiver sido enviada, uma solicitação para atualizar a tarefa retornará um erro.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Atualizando a ocorrência atual de uma tarefa recorrente

O resultado de uma operação UpdateItem em tarefas recorrentes difere do resultado da operação UpdateItem em uma única tarefa recorrente. Alterações a uma ocorrência de uma tarefa recorrente fazem com que as tarefas individuais sejam geradas quando as seguintes atualizações são feitas:
  
1. A propriedade status de uma tarefa regeradora ou nonregenerating recorrente está definida como **concluída**.
    
2. A data de início ou a data de término de uma tarefa recorrente de nonregenerating é alterada.
    
Por exemplo, se uma solicitação **UpdateItem** define o valor concluído de uma tarefa recorrente como **true**, o **UpdateItemResponse** incluirá uma nova ID e ChangeKey que representam uma tarefa única recém-criada. A ID que foi incluída na solicitação ainda é válida e a tarefa recorrente representada pela ID foi atualizada para representar a próxima ocorrência. O ChangeKey que foi incluído na solicitação não é mais válido porque a tarefa recorrente foi atualizada. 
  
Você pode usar a [operação GetItem](getitem-operation.md) para obter o **ChangeKey** mais recente para a tarefa recorrente. 
  
Para tarefas recorrentes ou para a última ocorrência de uma tarefa recorrente, a resposta UpdateItem retorna a mesma **ID** que foi passada e retorna a **ChangeKey**atualizada associada.
  
## <a name="see-also"></a>Confira também



[Operação UpdateItem](updateitem-operation.md)

