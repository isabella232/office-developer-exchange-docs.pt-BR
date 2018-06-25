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
description: O elemento de FindFolder define uma solicitação para localizar pastas em uma caixa de correio.
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752269"
---
# <a name="findfolder"></a>FindFolder

O elemento de **FindFolder** define uma solicitação para localizar pastas em uma caixa de correio. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 **FindFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Passagem  <br/> |Define como uma pesquisa é executada. Este atributo é necessário.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

|**Valor**|**Descrição**|
|:-----|:-----|
|Raso  <br/> |Instrui a operação FindFolder para pesquisar somente a pasta identificada e retornar somente a pasta IDs para itens que não foram excluídos. Isso é chamado uma passagem superficial.  <br/> |
|Profundo  <br/> |Instrui a operação FindFolder para pesquisar em todas as pastas filho da pasta pai identificados e retornar somente a pasta IDs para itens que não foram excluídos. Isso é chamado um percurso profundo.  <br/> |
|SoftDeleted  <br/> |Instrui a operação FindFolder para realizar uma pesquisa de passagem superficial para itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades de pasta para incluir em uma resposta FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Descreve como paginados informações de item são retornados em uma resposta FindFolder. Esse elemento é opcional.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Descreve o modo de exibição paginado inicia onde e o número máximo de pastas retornados em uma solicitação de FindFolder. Esse elemento é opcional.  <br/> |
|[Restriction](restriction.md) <br/> |Define uma restrição ou a consulta que é usada para filtrar as pastas em uma operação FindFolder. Esse elemento é opcional.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifica as pastas para a operação FindFolder pesquisar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação de FindFolder mostra como uma solicitação para localizar todas as pastas localizadas em uma caixa de entrada de formulário.
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindFolder](findfolder-operation.md)

