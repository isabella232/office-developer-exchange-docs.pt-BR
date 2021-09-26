---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: O elemento AlternatePublicFolderItemId descreve um identificador de item de pasta pública para converter em outro formato de identificador. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e3d71d17c6e9321a1accfbaf90967d2b504f5efe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543706"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

O **elemento AlternatePublicFolderItemId** descreve um identificador de item de pasta pública para converter em outro formato de identificador. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|FolderId  <br/> |Identifica a pasta pública que contém o item de pasta pública. Esse atributo é necessário.  <br/> |
|Formatar  <br/> |Identifica o formato que descreve o identificador de item de pasta pública a ser convertido. Esse atributo é necessário.  <br/> |
|ItemId  <br/> |Identifique o item de pasta pública a ser convertido. Esse atributo é necessário.  <br/> |
   
#### <a name="format-attribute-values"></a>Formatar valores de atributo

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
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a converter. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
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

