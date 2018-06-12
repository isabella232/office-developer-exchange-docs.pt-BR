---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: O elemento AlternatePublicFolderItemId descreve um identificador de item de pasta pública para converter em outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751086"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

O elemento **AlternatePublicFolderItemId** descreve um identificador de item de pasta pública para converter em outro formato de identificador. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|FolderId  <br/> |Identifica a pasta pública que contém o item de pasta pública. Este atributo é necessário.  <br/> |
|Format  <br/> |Identifica o formato que descreve o identificador de item de pasta pública para converter. Este atributo é necessário.  <br/> |
|ItemId  <br/> |Identificador do item de pasta pública para converter. Este atributo é necessário.  <br/> |
   
#### <a name="format-attribute-values"></a>Valores de atributos de formato

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
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem para converter. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
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

