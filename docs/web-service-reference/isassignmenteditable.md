---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: O elemento IsAssignmentEditable representa o tipo de tarefa.
ms.openlocfilehash: 91922c4d6abd4d88ac9e36dd3d4c0224fc1ee716
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823992"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

O elemento **IsAssignmentEditable** representa o tipo de tarefa. 
  
```xml
<IsAssignmentEditable/>
```

 **inteiro**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Esta propriedade é somente leitura. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|0  <br/> |O padrão para todos os itens de tarefa.  <br/> |
|1  <br/> |Uma solicitação de tarefa.  <br/> |
|2  <br/> |Aceitação de uma tarefa a partir de um destinatário de uma solicitação de tarefa.  <br/> |
|3  <br/> |Recusa de uma tarefa a partir de um destinatário de uma solicitação de tarefa.  <br/> |
|4  <br/> |Uma atualização para uma solicitação de tarefa anterior.  <br/> |
|5  <br/> |Não usado.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

