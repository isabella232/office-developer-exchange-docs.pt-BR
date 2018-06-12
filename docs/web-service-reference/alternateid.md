---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: O elemento AlternateId descreve um identificador para converter em uma solicitação e os resultados de um identificador convertido na resposta.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751080"
---
# <a name="alternateid"></a>AlternateId

O elemento **AlternateId** descreve um identificador para converter em uma solicitação e os resultados de um identificador convertido na resposta. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Descreve o identificador de origem em uma solicitação de [operação ConvertId](convertid-operation.md) e o identificador de destino em uma resposta de [operação ConvertId](convertid-operation.md) .  <br/> |
|Format  <br/> |Descreve o formato de fonte em uma solicitação de [operação ConvertId](convertid-operation.md) e o formato de destino em uma resposta de [operação ConvertId](convertid-operation.md) . O formato de destino é descrito pelo atributo **DestinationFormat** do elemento [ConvertId](convertid.md) na solicitação. Este atributo é do tipo **IdFormatType**.  <br/> |
|Mailbox  <br/> |Descreve o endereço Simple Mail Transfer Protocol (SMTP) da caixa de correio principal que contém os identificadores para converter.  <br/> |
|IsArchive  <br/> |Indica se o identificador representa uma pasta ou um item arquivado. Um valor **true** indica que o identificador representa uma pasta ou um item arquivado. Este atributo é opcional.  <br/> |
   
#### <a name="format-attribute-values"></a>Valores de atributos de formato

|**Valor**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |Descreve os identificadores que são produzidos pelo Exchange Web Services na versão inicial do Exchange 2007.  <br/> |
|EwsId  <br/> |Descreve os identificadores que são produzidos pelo Exchange Web Services começando com o Exchange 2007 SP1.  <br/> |
|EntryId  <br/> |Descreve os identificadores MAPI, como a propriedade **PR_ENTRYID** .  <br/> |
|HexEntryId  <br/> |Descreve uma representação hexadecimal codificado da propriedade **PR_ENTRYID** . Este é o formato de identificadores de eventos de calendário de disponibilidade.  <br/> |
|StoreId  <br/> |Descreve os identificadores de repositório do Exchange.  <br/> |
|OwaId  <br/> |Descreve um identificador do Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação ConvertId](convertid-operation.md) .  <br/> |
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem para converter.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O elemento **AlternateId** descreve os dois identificadores, o identificador de origem a ser convertido na solicitação de [operação ConvertId](convertid-operation.md) e o identificador convertido no elemento [ConvertIdResponse](convertidresponse.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

||||
|:-----|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ConvertId](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Convertendo identificadores](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

