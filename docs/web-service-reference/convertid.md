---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: O elemento ConvertId define uma solicitação para converter identificadores de item e pasta entre formatos Exchange com suporte. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: fe7d46697ba72ba6458136541488f5cd498169f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545556"
---
# <a name="convertid"></a>ConvertId

O **elemento ConvertId** define uma solicitação para converter identificadores de item e pasta entre formatos Exchange com suporte. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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
|**DestinationFormat** <br/> |Descreve o formato de identificador que será retornado para todos os identificadores convertidos. DestinationFormat é descrito pelo IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Atributo DestinationFormat

|**Valor**|**Descrição**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Representa o formato identificador usado para Exchange identificadores de Serviços Web fornecidos na versão inicial do Exchange 2007.  <br/> |
|**EwsId** <br/> |Representa o formato de identificador usado para Exchange identificadores do Web Services a partir Exchange Server 2007 SP1.  <br/> |
|**EntryId** <br/> |Representa o identificador MAPI, como na propriedade PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Representa o identificador de evento do calendário de disponibilidade. Esta é uma representação codificada por hexadecimal da propriedade PR_ENTRYID.  <br/> |
|**StoreId** <br/> |Representa o Exchange de armazenamento.  <br/> |
|**OwaId** <br/> |Representa o Outlook de identificador do Web Access.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a converter.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ConvertId](convertid-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

