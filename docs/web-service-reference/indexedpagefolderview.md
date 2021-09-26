---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: O elemento IndexedPageFolderView descreve como as informações de item paged são retornadas em uma resposta FindFolder.
ms.openlocfilehash: 0a5d0f7e63549b7a851862d957ff32dff4333ce3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542236"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

O **elemento IndexedPageFolderView** descreve como as informações de item paged são retornadas em uma [resposta FindFolder.](findfolder.md) 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de pastas a ser retornada na resposta. Esse atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento do **BasePoint**. O deslocamento deve ser maior ou igual a zero. Se **BasePoint** for igual a Beginning, o deslocamento será positivo. Se **BasePoint** for igual a End, o deslocamento será manipulado como se fosse negativo.  <br/> Isso identifica qual pasta será a primeira pasta entregue na resposta. Esse atributo é necessário.  <br/> |
|**BasePoint** <br/> |Descreve se a página de pastas será inicial ou final do conjunto de pastas encontradas com os critérios de pesquisa. Procurar desde o final sempre pesquisa para trás. Esse atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo BasePoint

|**Valor**|**Descrição**|
|:-----|:-----|
|Início  <br/> |O exibição paged começa no início do conjunto de pastas encontrado.  <br/> |
|End  <br/> |O exibição paged começa no final do conjunto de pastas encontrado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para encontrar pastas em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Comentários

Procurar do fim envolve mover para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa começará a partir de 75. Se 10 registros são retornados, o ponteiro é movido para trás e 10 registros adicionais para 65 e retorna os registros de 65 a 75. O próximo índice é 64. O próximo deslocamento do final para uma página é 100 menos 64, o que equivale a 36. O valor do próximo deslocamento do final para obter a próxima página indexada é 36.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

