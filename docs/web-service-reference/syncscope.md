---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: O elemento SyncScope especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização.
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463031"
---
# <a name="syncscope"></a>SyncScope

O elemento **SyncScope** especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |O elemento que define uma solicitação para sincronizar itens em uma pasta do repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/> /SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **SyncScope** . 
  
**Valores do elemento SyncScope**

|**Valor**|**Descrição**|
|:-----|:-----|
|NormalItems  <br/> |Especifica que somente os itens na pasta são retornados em uma resposta de sincronização.  <br/> |
|NormalAndAssociatedItems  <br/> |Especifica que os dois itens na pasta e as informações associadas à pasta são retornados em uma resposta de sincronização.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

