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
description: O elemento Alternateid descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta.
ms.openlocfilehash: 26df68bd814c2d323630c6bb40b4c31745017c71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527450"
---
# <a name="alternateid"></a>AlternateId

O elemento **alternateid** descreve um identificador a ser convertido em uma solicitação e os resultados de um identificador convertido na resposta. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Descreve o identificador de origem em uma solicitação de [operação convertid](convertid-operation.md) e descreve o identificador de destino em uma resposta de [operação convertid](convertid-operation.md) .  <br/> |
|Formatar  <br/> |Descreve o formato de origem em uma solicitação de [operação convertid](convertid-operation.md) e descreve o formato de destino em uma resposta de [operação convertid](convertid-operation.md) . O formato de destino é descrito pelo atributo **DestinationFormat** do elemento [convertid](convertid.md) na solicitação. Este atributo é do tipo **idformattype**.  <br/> |
|Caixa de correio  <br/> |Descreve o endereço SMTP (Simple Mail Transfer Protocol) principal da caixa de correio que contém os identificadores a serem convertidos.  <br/> |
|IsArchive  <br/> |Indica se o identificador representa um item ou pasta arquivada. Um valor **true** indica que o identificador representa um item ou uma pasta arquivada. Esse atributo é opcional.  <br/> |
   
#### <a name="format-attribute-values"></a>Valores de atributo de formato

|**Valor**|**Descrição**|
|:-----|:-----|
|EwsLegacyId  <br/> |Descreve os identificadores produzidos pelos serviços Web do Exchange na versão inicial de lançamento do Exchange 2007.  <br/> |
|EwsId  <br/> |Descreve os identificadores produzidos pelos serviços Web do Exchange a partir do Exchange 2007 SP1.  <br/> |
|EntryId  <br/> |Descreve os identificadores MAPI, como na propriedade **PR_ENTRYID** .  <br/> |
|HexEntryId  <br/> |Descreve uma representação codificada hexadecimal da propriedade **PR_ENTRYID** . Este é o formato de identificadores de eventos de calendário de disponibilidade.  <br/> |
|StoreId  <br/> |Descreve os identificadores de repositório do Exchange.  <br/> |
|OwaId  <br/> |Descreve um identificador do Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação convertid](convertid-operation.md) .  <br/> |
|[SourceIds](sourceids.md) <br/> |Contém os identificadores de origem a serem convertidos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O elemento **alternateid** descreve dois identificadores, o identificador de origem que deve ser convertido na solicitação de [operação convertid](convertid-operation.md) e o identificador convertido no elemento [ConvertIdResponse](convertidresponse.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

||||
|:-----|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação convertid](convertid-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Convertendo identificadores](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

