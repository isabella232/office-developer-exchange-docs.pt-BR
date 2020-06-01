---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: O elemento convertid define uma solicitação para converter o item e os identificadores de pasta entre os formatos compatíveis com o Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452535"
---
# <a name="convertid"></a>ConvertId

O elemento **convertid** define uma solicitação para converter o item e os identificadores de pasta entre os formatos compatíveis com o Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**DestinationFormat** <br/> |Descreve o formato de identificador que será retornado para todos os identificadores convertidos. O DestinationFormat é descrito pelo IdFormattype.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Atributo DestinationFormat

|**Valor**|**Descrição**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Representa o formato de identificador usado para os identificadores de serviços Web do Exchange fornecidos na versão inicial de lançamento do Exchange 2007.  <br/> |
|**EwsId** <br/> |Representa o formato de identificador usado para identificadores de serviços Web do Exchange a partir do Exchange Server 2007 SP1.  <br/> |
|**EntryId** <br/> |Representa o identificador MAPI, como na propriedade PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Representa o identificador de eventos do calendário de disponibilidade. Esta é uma representação codificada em hexadecimal da propriedade PR_ENTRYID.  <br/> |
|**StoreId** <br/> |Representa o identificador do repositório do Exchange.  <br/> |
|**OwaId** <br/> |Representa o formato de identificador do Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a serem convertidos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação convertid](convertid-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

