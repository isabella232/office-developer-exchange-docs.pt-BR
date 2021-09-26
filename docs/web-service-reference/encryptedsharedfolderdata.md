---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: O elemento EncryptedSharedFolderData contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes.
ms.openlocfilehash: c86f615e8936a379f465afab337a264d27238537
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546620"
---
# <a name="encryptedsharedfolderdata"></a>EncryptedSharedFolderData

O **elemento EncryptedSharedFolderData** contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes. 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 **EncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Token](token.md) <br/> |Contém dados criptografados que representam o token de identificação dos dados compartilhados.  <br/> |
|[Dados](data.md) <br/> |Contém dados criptografados que representam os dados compartilhados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) <br/> |Representa uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou dados de contato com outros clientes.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetSharingMetadata](getsharingmetadata-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

