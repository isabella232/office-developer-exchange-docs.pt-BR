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
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468051"
---
# <a name="isassignmenteditable"></a>IsAssignmentEditable

O elemento **IsAssignmentEditable** representa o tipo de tarefa. 
  
```xml
<IsAssignmentEditable/>
```

 **Semantic**
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
   
## <a name="text-value"></a>Valor de texto

Essa propriedade é somente leitura. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|,0  <br/> |O padrão para todos os itens de tarefa.  <br/> |
|1   <br/> |Uma solicitação de tarefa.  <br/> |
|duas  <br/> |Uma aceitação de tarefa de um destinatário de uma solicitação de tarefa.  <br/> |
|3D  <br/> |Um declínio de tarefa de um destinatário de uma solicitação de tarefa.  <br/> |
|4   <br/> |Uma atualização para uma solicitação de tarefa anterior.  <br/> |
|5   <br/> |Não usado.  <br/> |
   
## <a name="remarks"></a>Comentários

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

