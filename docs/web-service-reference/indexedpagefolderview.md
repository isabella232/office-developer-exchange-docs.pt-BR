---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: O elemento IndexedPageFolderView descreve como as informações de item paginado são retornadas em uma resposta FindFolder.
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457197"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

O elemento **IndexedPageFolderView** descreve como as informações de item paginado são retornadas em uma resposta [FindFolder](findfolder.md) . 
  
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
|**MaxEntriesReturned** <br/> |Descreve o número máximo de pastas a serem retornadas na resposta. Esse atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento do **BasePoint**. Offset deve ser maior ou igual a zero. Se **BasePoint** for igual a início, o deslocamento será positivo. Se **BasePoint** for igual a end, o deslocamento será tratado como se fosse negativo.  <br/> Isso identifica qual pasta será a primeira pasta entregue na resposta. Esse atributo é necessário.  <br/> |
|**BasePoint** <br/> |Descreve se a página de pastas será iniciada a partir do início ou do final do conjunto de pastas encontrado com os critérios de pesquisa. Procurar a partir do fim sempre pesquisa retroativamente. Esse atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo BasePoint

|**Valor**|**Descrição**|
|:-----|:-----|
|Extremidade  <br/> |O modo de exibição paginado começa no início do conjunto de pastas localizado.  <br/> |
|Final  <br/> |O modo de exibição paginado começa no final do conjunto de pastas encontrado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para localizar pastas em uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Comentários

Procurar de end envolve mover para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa iniciará de 75. Se 10 registros forem retornados, o ponteiro será movido para trás de 10 registros adicionais para 65 e retornará os registros 65 a 75. O próximo índice é 64. O próximo deslocamento do final de uma página é 100 menos 64, que é igual a 36. O valor do próximo deslocamento do fim para obter a próxima página indexada é 36.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

