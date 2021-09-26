---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: O elemento IsAssignmentEditable representa o tipo de tarefa.
ms.openlocfilehash: 10676cc8c6196a7294f3550856a47dce7d717e6a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544947"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

O **elemento IsAssignmentEditable** representa o tipo de tarefa. 
  
```xml
<IsAssignmentEditable/>
```

 **integer**
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
   
## <a name="text-value"></a>Valor de texto

Essa propriedade é somente leitura. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|0  <br/> |O padrão para todos os itens de tarefa.  <br/> |
|1  <br/> |Uma solicitação de tarefa.  <br/> |
|2  <br/> |Uma aceitação de tarefa de um destinatário de uma solicitação de tarefa.  <br/> |
|3  <br/> |Uma rebaixamento de tarefa de um destinatário de uma solicitação de tarefa.  <br/> |
|4   <br/> |Uma atualização para uma solicitação de tarefa anterior.  <br/> |
|5  <br/> |Não usado.  <br/> |
   
## <a name="remarks"></a>Comentários

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

