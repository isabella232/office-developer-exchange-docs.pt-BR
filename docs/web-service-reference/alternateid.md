---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: O elemento AlternateId descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta.
ms.openlocfilehash: 6346a45b48eb811cac705d8da85dc77e6c18262c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520938"
---
# <a name="alternateid"></a>AlternateId

O **elemento AlternateId** descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Descreve o identificador de origem em uma [solicitação](convertid-operation.md) de operação ConvertId e descreve o identificador de destino em uma resposta de [operação ConvertId.](convertid-operation.md)  <br/> |
|Formatar  <br/> |Descreve o formato de origem em uma [solicitação](convertid-operation.md) de operação ConvertId e descreve o formato de destino em uma resposta de [operação ConvertId.](convertid-operation.md) O formato de destino é descrito pelo **atributo DestinationFormat** do [elemento ConvertId](convertid.md) na solicitação. Esse atributo é do tipo **IdFormatType**.  <br/> |
|Mailbox  <br/> |Descreve o endereço SMTP (Simple Mail Transfer Protocol) principal da caixa de correio que contém os identificadores a ser traduzidos.  <br/> |
|IsArchive  <br/> |Indica se o identificador representa um item ou pasta arquivado. Um valor **true** indica que o identificador representa um item ou pasta arquivado. Esse atributo é opcional.  <br/> |
   
#### <a name="format-attribute-values"></a>Formatar valores de atributo

|**Valor**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |Descreve os identificadores que são produzidos pelos Serviços Web Exchange na versão inicial do Exchange 2007.  <br/> |
|EwsId  <br/> |Descreve identificadores que são produzidos pelos Serviços Web Exchange a partir do Exchange 2007 SP1.  <br/> |
|Entryid  <br/> |Descreve identificadores MAPI, como na propriedade **PR_ENTRYID.**  <br/> |
|HexEntryId  <br/> |Descreve uma representação codificada por hexadecimal da **propriedade PR_ENTRYID.** Esse é o formato dos identificadores de eventos do calendário de disponibilidade.  <br/> |
|StoreId  <br/> |Descreve os Exchange de armazenamento.  <br/> |
|OwaId  <br/> |Descreve um Outlook Web App identificador.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação ConvertId.](convertid-operation.md)  <br/> |
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a converter.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O **elemento AlternateId** descreve dois identificadores, o identificador de origem que deve ser convertido na solicitação de operação [ConvertId](convertid-operation.md) e o identificador convertido no [elemento ConvertIdResponse.](convertidresponse.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

||||
|:-----|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ConvertId](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

