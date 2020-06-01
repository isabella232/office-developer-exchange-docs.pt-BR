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
description: O elemento BaseShape identifica o conjunto de propriedades a ser retornado em uma resposta de item ou pasta.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464487"
---
# <a name="baseshape"></a>BaseShape

O elemento **BaseShape** identifica o conjunto de propriedades a ser retornado em uma resposta de item ou pasta. 
  
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
|[FolderShape](foldershape.md) <br/> | Identifica as propriedades da pasta a serem incluídas na resposta GetFolder, FindFolder ou SyncFolderHierarchy.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[Shape](itemshape.md) <br/> | Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. A tabela a seguir lista os possíveis valores de texto.
  
**Valores de texto para o elemento BaseShape**

|**Valor**|**Descrição**|
|:-----|:-----|
|IdOnly  <br/> |Retorna somente a ID do item ou da pasta.  <br/> |
|Padrão  <br/> |Retorna um conjunto de propriedades que são definidas como o padrão para o item ou pasta.  <br/> |
|Propriedades  <br/> |Retorna todas as propriedades usadas pela camada de lógica de negócios do Exchange para criar uma pasta.  <br/> |
   
A tabela a seguir lista as propriedades padrão que são retornadas para uma solicitação FindFolder. Todas as subpastas de uma determinada pasta são retornadas em ordem por nome.
  
**Propriedades padrão**

|**Folder**|**Propriedades padrão**|
|:-----|:-----|
|Caixa de Entrada  <br/> |FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas  <br/> |
|Contatos  <br/> |FolderId, nome para exibição, contagem total, contagem de subpastas  <br/> |
|Calendário  <br/> |FolderId, nome para exibição, contagem de subpastas  <br/> |
|Rascunhos  <br/> |FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas  <br/> |
|Itens excluídos  <br/> |FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas  <br/> |
|Outras pastas  <br/> |FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas  <br/> |
|Enviada  <br/> |FolderId, nome de exibição, contagem de não lidos, contagem total, contagem de subpastas  <br/> |
|Tarefas  <br/> |FolderId, nome de exibição, contagem atrasada, contagem total, contagem de subpastas  <br/> |
|Observações  <br/> |FolderId, nome para exibição, contagem total, contagem de subpastas  <br/> |
   
## <a name="remarks"></a>Comentários

Para retornar propriedades além daquelas identificadas pelo elemento [BaseShape](baseshape.md) , use o elemento Properties [adicionais](additionalproperties.md) . 
  
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
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [FolderShape](foldershape.md)
- [Shape](itemshape.md)

