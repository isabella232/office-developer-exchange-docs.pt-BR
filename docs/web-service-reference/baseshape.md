---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: O elemento BaseShape identifica o conjunto de propriedades a ser retornada em uma resposta de item ou pasta.
ms.openlocfilehash: b4e7f5c6d6520e7338f274b6275e371366b1bed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514855"
---
# <a name="baseshape"></a>BaseShape

O **elemento BaseShape** identifica o conjunto de propriedades a ser retornada em uma resposta de item ou pasta. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifica as propriedades de pasta a incluir na resposta GetFolder, FindFolder ou SyncFolderHierarchy.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. A tabela a seguir lista os valores de texto possíveis.
  
**Valores de texto para o elemento BaseShape**

|**Valor**|**Descrição**|
|:-----|:-----|
|IdOnly  <br/> |Retorna apenas o item ou a ID da pasta.  <br/> |
|Padrão  <br/> |Retorna um conjunto de propriedades que são definidas como padrão para o item ou pasta.  <br/> |
|AllProperties  <br/> |Retorna todas as propriedades usadas pela camada Exchange Business Logic para construir uma pasta.  <br/> |
   
A tabela a seguir lista as propriedades padrão retornadas para uma solicitação FindFolder. Todas as subpastas de uma determinada pasta são retornadas em ordem por nome.
  
**Propriedades padrão**

|**Folder**|**Propriedades padrão**|
|:-----|:-----|
|Caixa de Entrada  <br/> |FolderId, nome de exibição, contagem não lida, contagem total, contagem de subpastas  <br/> |
|Contatos  <br/> |FolderId, nome de exibição, contagem total, contagem de subpastas  <br/> |
|Calendário  <br/> |FolderId, nome de exibição, contagem de subpastas  <br/> |
|Rascunhos  <br/> |FolderId, nome de exibição, contagem não lida, contagem total, contagem de subpastas  <br/> |
|Itens excluídos  <br/> |FolderId, nome de exibição, contagem não lida, contagem total, contagem de subpastas  <br/> |
|Outras pastas  <br/> |FolderId, nome de exibição, contagem não lida, contagem total, contagem de subpastas  <br/> |
|Caixa de saída  <br/> |FolderId, nome de exibição, contagem não lida, contagem total, contagem de subpastas  <br/> |
|Tarefas  <br/> |FolderId, nome de exibição, contagem de vencimentos anteriores, contagem total, contagem de subpastas  <br/> |
|Observações  <br/> |FolderId, nome de exibição, contagem total, contagem de subpastas  <br/> |
   
## <a name="remarks"></a>Comentários

Para retornar propriedades além das identificadas pelo [elemento BaseShape,](baseshape.md) use o [elemento AdditionalProperties.](additionalproperties.md) 
  
## <a name="example"></a>Exemplo

```XML
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
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

