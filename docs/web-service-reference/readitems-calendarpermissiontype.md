---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: O elemento ReadItems indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824964"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

O elemento **ReadItems** indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Define o que um usuário tem acesso a uma pasta de calendário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **ReadItems** . 
  
**Valores de texto do elemento ReadItems**

|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Indica que o usuário não tem permissão para exibir itens do calendário.  <br/> |
|TimeOnly  <br/> |Indica que o usuário tem permissão para exibir o tempo de disponibilidade apenas no calendário.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indica que o usuário tem permissão para exibir o tempo de disponibilidade no calendário e o assunto e o local de compromissos.  <br/> |
|FullDetails  <br/> |Indica que o usuário tem permissão para exibir todos os itens do calendário, incluindo o tempo de livre/ocupado e assunto, local e detalhes dos compromissos.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões de nível de pasta](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

