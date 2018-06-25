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
description: O elemento IndexedPageFolderView descreve como paginados informações de item são retornados em uma resposta FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823910"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

O elemento **IndexedPageFolderView** descreve como paginados informações de item são retornados em uma resposta [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de pastas para retornar na resposta. Este atributo é opcional.  <br/> |
|**Offset** <br/> |Descreve o deslocamento, desde o **ponto de base**. Deslocamento deve ser maior ou igual a zero. Se o **ponto de base** é igual ao início, o deslocamento for positivo. Se o **ponto de base** for igual ao fim, o deslocamento é tratado como se fosse negativo.  <br/> Isso identifica a pasta na qual será a primeira pasta entregue na resposta. Este atributo é necessário.  <br/> |
|**Ponto de base** <br/> |Descreve como se a página de pastas será iniciado a partir do início ou no final do conjunto de pastas que são localizadas com os critérios de pesquisa. Procurando a partir do término do sempre pesquisa para trás. Este atributo é necessário.  <br/> |
   
#### <a name="basepoint-attribute"></a>Atributo de ponto de base

|**Valor**|**Descrição**|
|:-----|:-----|
|Início  <br/> |O modo de exibição paginado começa no início do conjunto de pasta encontrado.  <br/> |
|End  <br/> |O modo de exibição paginado inicia no final do conjunto de pasta encontrado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para localizar pastas em uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Comentários

Buscando a partir do término envolve mover para a origem identificada pelo deslocamento. Além disso, o ponteiro é movido de volta pelo número de registros solicitados. Por exemplo, se existem 100 registros e o deslocamento for 25 do fim, a pesquisa começa a partir 75. Se 10 registros forem retornados, o ponteiro é movido para trás uma 10 adicionais registra como 65 e retorna registros 65 por meio de 75. O próximo índice é 64. O deslocamento próximo do final de uma página é 100 menos 64 que é igual a 36. O valor para o próximo deslocamento do final para obter a próxima página indexada é 36.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

