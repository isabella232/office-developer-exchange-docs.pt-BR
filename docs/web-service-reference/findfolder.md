---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: O elemento FindFolder define uma solicitação para encontrar pastas em uma caixa de correio.
ms.openlocfilehash: 431efde28e417efec04f6fa1625a81b3766cb705
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518439"
---
# <a name="findfolder"></a>FindFolder

O **elemento FindFolder** define uma solicitação para encontrar pastas em uma caixa de correio. 
  
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
|Traversal  <br/> |Define como uma pesquisa é realizada. Esse atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores do atributo traversal

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Instrui a operação FindFolder a pesquisar somente a pasta identificada e retornar apenas as IDs de pasta para itens que não foram excluídos. Isso é chamado de uma transição superficial.  <br/> |
|Deep  <br/> |Instrui a operação FindFolder a pesquisar em todas as pastas filho da pasta pai identificada e retornar apenas as IDs de pasta para itens que não foram excluídos. Isso é chamado de uma transição profunda.  <br/> |
|SoftDeleted  <br/> |Instrui a operação FindFolder a executar uma pesquisa superficial em busca de itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades da pasta a incluir em uma resposta FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Descreve como as informações de item paged são retornadas em uma resposta FindFolder. Esse elemento é opcional.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Descreve onde o exibição paged é iniciado e o número máximo de pastas retornadas em uma solicitação FindFolder. Esse elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define uma restrição ou consulta usada para filtrar pastas em uma operação FindFolder. Esse elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica pastas para a operação FindFolder a ser pesquisada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação FindFolder mostra como formar uma solicitação para localizar todas as pastas localizadas em uma Caixa de Entrada.
  
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

