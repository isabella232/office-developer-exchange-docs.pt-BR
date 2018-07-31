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
description: O elemento ParentFolderId identifica a pasta na qual uma nova pasta é criada ou a pasta para pesquisar a operação FindConversation.
ms.openlocfilehash: 8e80b9b342274a8b2004838ebd16f8425a2d3fa3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353823"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

O elemento **ParentFolderId** identifica a pasta na qual uma nova pasta é criada ou a pasta para pesquisar a [operação FindConversation](findconversation-operation.md).
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

O elemento **ParentFolderId** contém dois elementos filho. Os elementos filhos são mutuamente exclusivos no esquema. 
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador necessário e a chave de alteração opcionais de uma pasta na qual uma nova pasta é criada ou a pasta que será pesquisada para a [operação FindConversation](findconversation-operation.md). Usar esse elemento exclui o uso do elemento [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica as pastas padrão do Microsoft Exchange Server 2007. Usar esse elemento exclui o uso do elemento [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Define uma solicitação para criar uma pasta do banco de dados do Exchange.  <br/> Este é a expressão XPath para esse elemento:`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Define uma solicitação para localizar conversas em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

Os elementos dois filhos são usados para definir a pasta que conterá a nova pasta. Você deve selecionar o [FolderId](folderid.md) ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) para identificar a pasta pai da nova pasta. Você não pode usar ambos os elementos ao mesmo tempo. Esse elemento é necessário para criar pastas. 
  
O elemento [ParentFolderId](parentfolderid.md) descreve a localização de itens e pastas existentes. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação CreateFolder](createfolder-operation.md)
- [Operação FindConversation](findconversation-operation.md)
- [Criação de pastas (serviços Web do Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

