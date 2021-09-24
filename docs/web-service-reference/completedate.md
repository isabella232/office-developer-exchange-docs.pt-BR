---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: O elemento CompleteDate representa a data em que um item foi concluído.
ms.openlocfilehash: 07f6034b4fd91d22ad07167d931bcd02a74782f9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518775"
---
# <a name="completedate"></a>CompleteDate

O **elemento CompleteDate** representa a data em que um item foi concluído. 
  
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
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[Flag](flag.md) <br/> |Especifica um sinalizador em um item de caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa a data e a hora é necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

Definir **CompleteDate** tem o mesmo efeito que definir [PercentComplete](percentcomplete.md) como 100 ou [Status](status.md) como **Concluído.** Em uma solicitação que define pelo menos duas dessas propriedades, a última propriedade processada determinará o valor definido para esses elementos. Por exemplo, se [PercentComplete](percentcomplete.md) for 100, **CompleteDate** for 1º de janeiro de 2007 e Status for **NotStarted**, e as propriedades são transmitidas nessa ordem, o efeito será definir [o Status](status.md) da tarefa como **NotStarted**, [CompleteDate](completedate.md) como nulo **e** [PercentComplete](percentcomplete.md) como 0. [](status.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Excluir Tarefas](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

