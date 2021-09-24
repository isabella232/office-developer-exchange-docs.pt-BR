---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: O elemento SyncScope especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização.
ms.openlocfilehash: 5e5d19809cea1f8f244444c09615ee888fea05be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538895"
---
# <a name="syncscope"></a>SyncScope

O **elemento SyncScope** especifica se apenas itens ou itens e informações associadas à pasta são retornados em uma resposta de sincronização. 
  
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
|[SyncFolderItems](syncfolderitems.md) <br/> |O elemento que define uma solicitação para sincronizar itens em uma Exchange de armazenamento.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/> /SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento SyncScope.** 
  
**Valores do elemento SyncScope**

|**Valor**|**Descrição**|
|:-----|:-----|
|NormalItems  <br/> |Especifica que apenas os itens na pasta são retornados em uma resposta de sincronização.  <br/> |
|NormalAndAssociatedItems  <br/> |Especifica que os itens na pasta e nas informações associadas à pasta são retornados em uma resposta de sincronização.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
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

