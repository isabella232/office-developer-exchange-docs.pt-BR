---
title: Concluído
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: O elemento CompleteD representa a data em que um item foi concluído.
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461419"
---
# <a name="completedate"></a>Concluído

O elemento **Completed** representa a data em que um item foi concluído. 
  
```xml
<CompleteDate/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[Flag](flag.md) <br/> |Especifica um sinalizador em um item de caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa a data e hora é necessário se esse elemento é usado.
  
## <a name="remarks"></a>Comentários

A configuração foi **concluída** tem o mesmo efeito que configurar a [PorcentagemConcluída](percentcomplete.md) como 100 ou [status](status.md) como **concluído**. Em uma solicitação que define pelo menos duas dessas propriedades, a última Propriedade processada determinará o valor definido para esses elementos. Por exemplo, se [a PorcentagemConcluída](percentcomplete.md) for 100, **Completed** for 1 de janeiro de 2007, e o [status](status.md) não for **iniciado**e as propriedades forem transmitidas nessa ordem, o efeito será definir o [status](status.md) da tarefa como não **iniciada**, [concluída](completedate.md) como **nulo**e [PorcentagemConcluída](percentcomplete.md) como 0. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Excluir tarefas](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

