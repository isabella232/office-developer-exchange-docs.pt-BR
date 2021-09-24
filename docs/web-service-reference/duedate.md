---
title: DueDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DueDate
api_type:
- schema
ms.assetid: dd9b6c43-a512-4b3b-a071-4abde02ed55f
description: O elemento DueDate representa a data de vencimento de um item.
ms.openlocfilehash: 039008ae2ceb2faf280c5b434a5068b580ee885c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540079"
---
# <a name="duedate"></a>DueDate

O **elemento DueDate** representa a data de vencimento de um item. 
  
```xml
<DueDate/>
```

 **dateTime**
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

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

