---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: O elemento GetItem define uma solicitação para obter um item de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: a02403ee84195a41387d5dbe1785ae6d12b47da5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458695"
---
# <a name="getitem"></a>GetItem

O elemento **GetItem** define uma solicitação para obter um item de uma caixa de correio no repositório do Exchange. 
  
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
|[Shape](itemshape.md) <br/> |Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta **GetItem** .  <br/> |
|[ItemIds](itemids.md) <br/> |Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes que são usados para obter itens do repositório do Exchange. Estes itens representam contatos, tarefas, mensagens, itens de calendário, solicitações de reunião e outros itens válidos em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
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

