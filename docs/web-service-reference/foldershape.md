---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: O elemento FolderShape identifica as propriedades de pasta a incluir em uma resposta GetFolder, FindFolder ou SyncFolderHierarchy.
ms.openlocfilehash: 530c9f25f17a3eba8549535bf7be37038a58c921
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518355"
---
# <a name="foldershape"></a>FolderShape

O **elemento FolderShape** identifica as propriedades de pasta a incluir em uma resposta [GetFolder,](getfolder.md) [FindFolder](findfolder.md)ou [SyncFolderHierarchy.](syncfolderhierarchy.md) 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **FolderResponseShapeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifica a configuração básica das propriedades a ser retornada em uma resposta.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais para retornar em uma resposta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Define uma solicitação para obter uma pasta do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Define uma solicitação para sincronizar uma hierarquia de pastas em um cliente.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento FolderShape** é um elemento filho necessário do [elemento FindFolder.](findfolder.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação demonstra como localizar todas as pastas localizadas no primeiro nível da pasta Caixa de Entrada.
  
```
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



[FindFolder](findfolder.md)

