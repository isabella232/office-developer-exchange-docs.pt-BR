---
title: FolderNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: O elemento FolderNames contém uma matriz de pastas gerenciadas nomeadas para adicionar a uma caixa de correio.
ms.openlocfilehash: be9b11ca9ca9c81914082f26ee61dbcd1990e9f6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530294"
---
# <a name="foldernames"></a>FolderNames

O **elemento FolderNames** contém uma matriz de pastas gerenciadas nomeadas para adicionar a uma caixa de correio. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 **NonEmptyArrayOfFolderNamesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderName](foldername.md) <br/> |Identifica uma única pasta gerenciada para adicionar à caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateManagedFolder](createmanagedfolder.md) <br/> |O elemento raiz em uma solicitação para adicionar uma pasta gerenciada a uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindFolder](findfolder-operation.md)


[Localizar Pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

