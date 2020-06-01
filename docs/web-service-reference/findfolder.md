---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: O elemento FindFolder define uma solicitação para localizar pastas em uma caixa de correio.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462574"
---
# <a name="findfolder"></a>FindFolder

O elemento **FindFolder** define uma solicitação para localizar pastas em uma caixa de correio. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

**FindFolderType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Passagem  <br/> |Define como uma pesquisa é realizada. Esse atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Instrui a operação FindFolder a pesquisar somente a pasta identificada e retornar apenas as IDs de pasta para itens que não foram excluídos. Isso é chamado de passagem superficial.  <br/> |
|Detalhadas  <br/> |Instrui a operação FindFolder para pesquisar em todas as pastas filhas da pasta pai identificada e para retornar apenas as IDs de pasta para itens que não foram excluídos. Isso é chamado de passagem profunda.  <br/> |
|SoftDeleted  <br/> |Instrui a operação FindFolder a realizar uma pesquisa de passagem superficial para itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades da pasta a serem incluídas em uma resposta FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Descreve como as informações de item paginado são retornadas em uma resposta FindFolder. Este elemento é opcional.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação FindFolder. Este elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define uma restrição ou consulta usada para filtrar pastas em uma operação FindFolder. Este elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica pastas para a operação FindFolder a ser pesquisada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação FindFolder mostra como formar uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindFolder](findfolder-operation.md)

