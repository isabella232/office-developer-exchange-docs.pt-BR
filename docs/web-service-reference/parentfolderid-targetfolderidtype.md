---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: O elemento ParentFolderId identifica a pasta na qual uma nova pasta é criada ou a pasta a ser pesquisada para a operação FindConversation.
ms.openlocfilehash: 53a5721b2c20c211a61b7e71b2e4f636700456b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524620"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

O **elemento ParentFolderId** identifica a pasta na qual uma nova pasta é criada ou a pasta a ser pesquisada para a [operação FindConversation](findconversation-operation.md).
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Atributos e elementos

O **elemento ParentFolderId** contém dois elementos filho. Os elementos filho são mutuamente exclusivos no esquema. 
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador necessário e a chave de alteração opcional de uma pasta na qual uma nova pasta é criada ou a pasta pesquisada para a operação [FindConversation](findconversation-operation.md). O uso desse elemento exclui o uso do [elemento DistinguishedFolderId.](distinguishedfolderid.md)  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas Microsoft Exchange Server 2007 padrão. O uso desse elemento exclui o uso do [elemento FolderId.](folderid.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Define uma solicitação para criar uma pasta no banco Exchange banco de dados.  <br/> Veja a seguir a expressão XPath para este elemento:  `/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para encontrar conversas em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Os dois elementos filho são usados para definir a pasta que conterá a nova pasta. Você deve selecionar [FolderId](folderid.md) ou [o elemento DistinguishedFolderId](distinguishedfolderid.md) para identificar a pasta pai da nova pasta. Não é possível usar ambos os elementos ao mesmo tempo. Esse elemento é necessário para criar pastas. 
  
O [elemento ParentFolderId](parentfolderid.md) descreve o local de itens e pastas existentes. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação CreateFolder](createfolder-operation.md)
- [Operação FindConversation](findconversation-operation.md)
- [Criando Pastas (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

