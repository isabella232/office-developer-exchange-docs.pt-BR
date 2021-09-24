---
title: Operação UpdateItem (tarefa)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: A operação UpdateItem é usada para atualizar as propriedades do item de tarefa no Exchange store.
ms.openlocfilehash: a268b4b281f149f14bc6c48a774fc9071093ebb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510747"
---
# <a name="updateitem-operation-task"></a>Operação UpdateItem (tarefa)

A operação UpdateItem é usada para atualizar as propriedades do item de tarefa no Exchange store.
  
## <a name="remarks"></a>Comentários

Você não pode usar Exchange Web Services para enviar solicitações de tarefa. Exchange Os Serviços Web podem retornar solicitações de tarefas criadas pelo MicrosoftOfficeOutlook. Se uma solicitação de tarefa já tiver sido enviada, uma solicitação para atualizar a tarefa retornará um erro.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Atualizando a Ocorrência Atual de uma Tarefa Recorrente

O resultado de uma operação UpdateItem em tarefas recorrentes difere do resultado da operação UpdateItem em uma única tarefa não recorrente. As alterações em uma ocorrência de uma tarefa recorrente fazem com que tarefas simples sejam geradas quando as seguintes atualizações são feitas:
  
1. A propriedade status de uma tarefa recorrente regenerante ou não recorrente é definida como **Concluída**.
    
2. A data de início ou a data de término de uma tarefa recorrente não recorrente é alterada.
    
Por exemplo, se uma solicitação **UpdateItem** define o valor Concluído de uma tarefa recorrente como **true**, **UpdateItemResponse** incluirá uma nova Id e ChangeKey que representam uma tarefa única recém-criada. A ID incluída na solicitação ainda é válida e a tarefa recorrente representada por essa ID foi atualizada para representar a próxima ocorrência. O ChangeKey incluído na solicitação não é mais válido porque a tarefa recorrente foi atualizada. 
  
Você pode usar a [operação GetItem](getitem-operation.md) para obter o **ChangeKey mais** recente para a tarefa recorrente. 
  
Para tarefas não recorrentes ou para a última ocorrência de uma tarefa recorrente, a resposta UpdateItem retorna a mesma **ID** que foi passada para ela e retorna a **ChangeKey atualizada associada.**
  
## <a name="see-also"></a>Confira também



[Operação UpdateItem](updateitem-operation.md)

