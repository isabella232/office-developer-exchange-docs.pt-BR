---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: O elemento AlternatePublicFolderId descreve um identificador de pasta pública para converter em outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 32e6e75eb381e479baf5fdb5ad0a40b32c1b02a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751087"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

O elemento **AlternatePublicFolderId** descreve um identificador de pasta pública para converter em outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|FolderId  <br/> |Contém o identificador de pasta pública para converter. Este atributo é necessário.  <br/> |
|Format  <br/> |Identifica o formato que descreve o identificador de pasta pública para converter. Este atributo é necessário.  <br/> |
   
#### <a name="format-attribute"></a>Atributo Format

|**Valor**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |Descreve os identificadores que são produzidos pelo Exchange Web Services na versão inicial do Exchange 2007.  <br/> |
|EwsId  <br/> |Descreve os identificadores que são produzidos pelo Exchange Web Services começando com o Exchange 2007 SP1.  <br/> |
|EntryId  <br/> |Descreve os identificadores MAPI, como a propriedade PR_ENTRYID.  <br/> |
|HexEntryId  <br/> |Descreve uma representação hexadecimal codificado da propriedade PR_ENTRYID. Este é o formato de identificadores de eventos de calendário de disponibilidade.  <br/> |
|StoreId  <br/> |Descreve os identificadores de repositório do Exchange.  <br/> |
|OwaId  <br/> |Descreve um identificador do Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem para converter. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ConvertId](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Convertendo identificadores](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

