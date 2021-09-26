---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: O elemento GetItem define uma solicitação para obter um item de uma caixa de correio no Exchange store.
ms.openlocfilehash: 7d5a7253db54fd67bb8e8772c2a5aedb86abdeee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546228"
---
# <a name="getitem"></a>GetItem

O **elemento GetItem** define uma solicitação para obter um item de uma caixa de correio no Exchange store. 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 **GetItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma **resposta GetItem.**  <br/> |
|[ItemIds](itemids.md) <br/> |Contém as identidades exclusivas de itens, itens de ocorrência e itens mestras recorrentes que são usados para obter itens do Exchange store. Esses itens representam contatos, tarefas, mensagens, itens de calendário, solicitações de reunião e outros itens válidos em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetItem](getitem-operation.md)

