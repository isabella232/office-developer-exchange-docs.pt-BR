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
description: O elemento de ConvertId define uma solicitação para converter os identificadores de item e pasta entre formatos suportados do Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751535"
---
# <a name="convertid"></a>ConvertId

O elemento de **ConvertId** define uma solicitação para converter os identificadores de item e pasta entre formatos suportados do Exchange. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**DestinationFormat** <br/> |Descreve o formato do identificador que será retornado para todos os identificadores convertidos. O DestinationFormat é descrito pelo IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Atributo DestinationFormat

|**Valor**|**Descrição**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Representa o formato do identificador que é usado para os identificadores de serviços Web do Exchange que são fornecidos na versão inicial do Exchange 2007.  <br/> |
|**EwsId** <br/> |Representa o formato do identificador que é usado para identificadores de serviços Web do Exchange, começando com o Exchange Server 2007 SP1.  <br/> |
|**EntryId** <br/> |Representa o identificador MAPI, como a propriedade PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Representa o identificador de eventos de calendário de disponibilidade. Esta é uma representação hexadecimal codificado da propriedade PR_ENTRYID.  <br/> |
|**StoreId** <br/> |Representa o identificador de repositório do Exchange.  <br/> |
|**OwaId** <br/> |Representa o formato de identificador do Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem para converter.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação ConvertId](convertid-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Convertendo identificadores](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

