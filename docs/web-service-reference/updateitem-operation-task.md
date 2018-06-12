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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837912"
---
# <a name="updateitem-operation-task"></a>Operação UpdateItem (tarefa)

A operação UpdateItem é usada para atualizar as propriedades de item de tarefa no armazenamento do Exchange.
  
## <a name="remarks"></a>Coment�rios

Você não pode usar os serviços Web do Exchange para enviar solicitações de tarefa. Serviços Web do Exchange pode retornar as solicitações de tarefa que são criadas por MicrosoftOfficeOutlook. Se já tiver sido enviada a uma solicitação de tarefa, uma solicitação para atualizar a tarefa retornará um erro.
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a>Atualizando a ocorrência atual de uma tarefa recorrente

O resultado de uma operação de UpdateItem em tarefas recorrentes difere do resultado da operação UpdateItem sobre uma tarefa única e nonrecurring. Alterações em uma ocorrência de uma tarefa recorrente causar únicas tarefas a serem gerados quando as seguintes atualizações são feitas:
  
1. A propriedade do status de uma tarefa recorrente regeneração ou nonregenerating é definida como **concluído**.
    
2. A data de início ou data de término de uma tarefa recorrente nonregenerating é alterada.
    
Por exemplo, se uma solicitação de **UpdateItem** define o valor de concluído de uma tarefa recorrente como **true**, o **UpdateItemResponse** incluirá uma nova Id e ChangeKey que representam uma tarefa único recém-criado. A Id que foi incluída na solicitação ainda é válida e a tarefa recorrente que é representada por esse Id foi atualizada para representar a próxima ocorrência. O que foi incluída na solicitação ChangeKey não é mais válido porque a tarefa recorrente foi atualizada. 
  
Você pode usar a [operação GetItem](getitem-operation.md) para obter as últimas **ChangeKey** para a tarefa recorrente. 
  
Para tarefas nonrecurring ou a última ocorrência de uma tarefa recorrente, a resposta UpdateItem retorna a mesma **Id** que foi passado para ele e retorna que o associado atualizado **ChangeKey**.
  
## <a name="see-also"></a>Confira também



[Operação UpdateItem](updateitem-operation.md)

