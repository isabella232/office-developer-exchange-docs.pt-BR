---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: O elemento EncryptedSharedFolderData contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752043"
---
# <a name="encryptedsharedfolderdata"></a>EncryptedSharedFolderData

O elemento **EncryptedSharedFolderData** contém os dados criptografados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes. 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 **EncryptedSharedFolderDataType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Token](token.md) <br/> |Contém os dados criptografados que representa o token de identificação para os dados compartilhados.  <br/> |
|[Data](data.md) <br/> |Contém os dados criptografados que representa os dados compartilhados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) <br/> |Representa uma coleção de estruturas de dados que um cliente pode usar para autorizar o compartilhamento de seu calendário ou entre em contato com o serviço de dados com outros clientes.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetSharingMetadata](getsharingmetadata-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

