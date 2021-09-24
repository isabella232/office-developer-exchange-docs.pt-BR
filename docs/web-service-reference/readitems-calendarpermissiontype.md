---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: O elemento ReadItems indica se um usuário tem permissão para ler itens em uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a12b5316eaebfdf6d0d70468f172f227db7ab3ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519083"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

O **elemento ReadItems** indica se um usuário tem permissão para ler itens em uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Define o acesso que um usuário tem a uma pasta Calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento ReadItems.** 
  
**Valores de texto do elemento ReadItems**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o usuário não tem permissão para exibir itens no calendário.  <br/> |
|TimeOnly  <br/> |Indica que o usuário tem permissão para exibir somente o horário de trabalho no calendário.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indica que o usuário tem permissão para exibir o tempo livre/ocupado no calendário e o assunto e o local dos compromissos.  <br/> |
|FullDetails  <br/> |Indica que o usuário tem permissão para exibir todos os itens no calendário, incluindo horário de livre/ocupado e assunto, local e detalhes de compromissos.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

