---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: O elemento AlternatePublicFolderId descreve um identificador de pasta pública para converter em outro formato de identificador. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7c4471c0c1e3e1eee3b47eba42f924340891c777
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525355"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

O **elemento AlternatePublicFolderId** descreve um identificador de pasta pública para converter em outro formato de identificador. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|FolderId  <br/> |Contém o identificador de pasta pública a ser convertido. Esse atributo é necessário.  <br/> |
|Formatar  <br/> |Identifica o formato que descreve o identificador de pasta pública a ser convertido. Esse atributo é necessário.  <br/> |
   
#### <a name="format-attribute"></a>Atributo Format

|**Valor**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |Descreve os identificadores que são produzidos pelos Serviços Web Exchange na versão inicial do Exchange 2007.  <br/> |
|EwsId  <br/> |Descreve identificadores que são produzidos pelos Serviços Web Exchange a partir do Exchange 2007 SP1.  <br/> |
|Entryid  <br/> |Descreve identificadores MAPI, como na propriedade PR_ENTRYID.  <br/> |
|HexEntryId  <br/> |Descreve uma representação codificada por hexadecimal da propriedade PR_ENTRYID. Esse é o formato dos identificadores de eventos do calendário de disponibilidade.  <br/> |
|StoreId  <br/> |Descreve os Exchange de armazenamento.  <br/> |
|OwaId  <br/> |Descreve um identificador Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a converter. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ConvertId](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

