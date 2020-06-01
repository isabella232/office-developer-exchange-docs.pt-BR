---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: O elemento ParentFolderId identifica a pasta na qual uma nova pasta é criada ou a pasta a ser pesquisada para a operação FindConversation.
ms.openlocfilehash: 36e63266d10603c4d453a37e2b0d22e02599e516
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467799"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

O elemento **ParentFolderId** identifica a pasta na qual uma nova pasta é criada ou a pasta a ser pesquisada para a [operação FindConversation](findconversation-operation.md).
  
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

O elemento **ParentFolderId** contém dois elementos filhos. Os elementos filho são mutuamente exclusivos no esquema. 
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador necessário e a chave de alteração opcional de uma pasta na qual uma nova pasta é criada ou a pasta que é pesquisada para a [operação FindConversation](findconversation-operation.md). O uso deste elemento exclui o uso do elemento [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas padrão do Microsoft Exchange Server 2007. O uso deste elemento exclui o uso do elemento [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Define uma solicitação para criar uma pasta no banco de dados do Exchange.  <br/> A seguir está a expressão XPath para este elemento:`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para encontrar conversas em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Os dois elementos filhos são usados para definir a pasta que conterá a nova pasta. Você deve selecionar o elemento [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) para identificar a pasta pai da nova pasta. Você não pode usar ambos os elementos ao mesmo tempo. Esse elemento é necessário para criar pastas. 
  
O elemento [ParentFolderId](parentfolderid.md) descreve o local das pastas e itens existentes. 
  
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
- [Criando pastas (serviços Web do Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

