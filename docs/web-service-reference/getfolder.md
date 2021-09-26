---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: O elemento GetFolder define uma solicitação para obter uma pasta de uma caixa de correio no Exchange store.
ms.openlocfilehash: dc6004a05bce51592dbc6e4e7df6993821951e50
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546291"
---
# <a name="getfolder"></a>GetFolder

O **elemento GetFolder** define uma solicitação para obter uma pasta de uma caixa de correio no Exchange store. 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 **GetFolderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades a obter para cada pasta identificada no [elemento FolderIds.](folderids.md)  <br/> |
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para obter de uma caixa de correio no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
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



[Operação GetFolder](getfolder-operation.md)

