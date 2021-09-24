---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: O elemento SharingFolderId representa o identificador da pasta local em um relacionamento de compartilhamento.
ms.openlocfilehash: 9f26efa394341c8ead895a1d8e898cb48d9c2cb9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540437"
---
# <a name="sharingfolderid"></a>SharingFolderId

O **elemento SharingFolderId** representa o identificador da pasta local em um relacionamento de compartilhamento. 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Contém uma cadeia de caracteres que identifica uma pasta no Exchange store. Esse atributo é necessário.  <br/> |
|ChangeKey  <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo Id. Esse atributo é opcional. Use esse atributo para garantir que a versão correta de uma pasta seja usada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |Define uma solicitação para atualizar a pasta local especificada.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação [GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

