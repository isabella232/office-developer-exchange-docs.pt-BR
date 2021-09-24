---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: O elemento EncryptedSharedFolderDataCollection contém uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes.
ms.openlocfilehash: 868bff4e1afc905196bd4c48eba966cb8b7b08a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540073"
---
# <a name="encryptedsharedfolderdatacollection"></a>EncryptedSharedFolderDataCollection

O **elemento EncryptedSharedFolderDataCollection** contém uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes. 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 **ArrayOfEncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EncryptedSharedFolderData](encryptedsharedfolderdata.md) <br/> |Contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação [GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
   
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

- [Operação GetSharingMetadata](getsharingmetadata-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

