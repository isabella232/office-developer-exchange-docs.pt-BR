---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: O elemento OriginalRecipients representa uma lista de endereços de email dos destinatários da primeira mensagem.
ms.openlocfilehash: 38066a14cbac02ead7e56cef3d448509302d545d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546137"
---
# <a name="originalrecipients"></a>OriginalRecipients

O **elemento OriginalRecipients** representa uma lista de endereços de email dos destinatários da primeira mensagem. 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 **ArrayOfEmailAddressesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Address (EmailAddressType)](address-emailaddresstype.md) <br/> |Contém um endereço de email totalmente resolvido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contém uma única mensagem retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

