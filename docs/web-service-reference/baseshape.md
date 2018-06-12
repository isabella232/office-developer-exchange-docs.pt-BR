---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: O elemento BaseShape identifica o conjunto de propriedades para retornar em uma resposta de item ou uma pasta.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751265"
---
# <a name="baseshape"></a>BaseShape

O elemento **BaseShape** identifica o conjunto de propriedades para retornar em uma resposta de item ou uma pasta. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

None
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifica as propriedades de pasta para incluir na resposta GetFolder, FindFolder ou SyncFolderHierarchy.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.<br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. A tabela a seguir lista os valores de texto possíveis.
  
**Valores de texto para o elemento BaseShape**

|**Valor**|**Descrição**|
|:-----|:-----|
|IdOnly  <br/> |Retorna apenas o ID de item ou uma pasta  <br/> |
|Default  <br/> |Retorna um conjunto de propriedades que são definidas como padrão para o item ou a pasta.  <br/> |
|AllProperties  <br/> |Retorna todas as propriedades utilizadas pela camada de lógica de negócios do Exchange para construir uma pasta.  <br/> |
   
A tabela a seguir lista as propriedades padrão que são retornadas para uma solicitação de FindFolder. Todas as subpastas de uma determinada pasta são retornadas em ordem pelo nome.
  
**Propriedades padrão**

|**Folder**|**Propriedades padrão**|
|:-----|:-----|
|Caixa de Entrada  <br/> |FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta  <br/> |
|Contatos  <br/> |FolderId, nome para exibição, a contagem total, a contagem de subpasta  <br/> |
|Calendário  <br/> |FolderId, nome para exibição, contagem da subpasta  <br/> |
|Rascunhos  <br/> |FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta  <br/> |
|Itens excluídos  <br/> |FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta  <br/> |
|Outras pastas  <br/> |FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta  <br/> |
|Caixa de saída  <br/> |FolderId, nome para exibição, contagem não lida, contagem total, contagem da subpasta  <br/> |
|Tarefas  <br/> |FolderId, nome para exibição, vencidos contagem, a contagem total, a contagem de subpasta  <br/> |
|Observações  <br/> |FolderId, nome para exibição, a contagem total, a contagem de subpasta  <br/> |
   
## <a name="remarks"></a>Coment�rios

Para retornar propriedades além daquelas identificado pelo elemento [BaseShape](baseshape.md) , use o elemento [AdditionalProperties](additionalproperties.md) . 
  
## <a name="example"></a>Example

```XML
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
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

