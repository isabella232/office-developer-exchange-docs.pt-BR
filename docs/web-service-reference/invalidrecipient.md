---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: O elemento InvalidRecipient contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.
ms.openlocfilehash: 507cdf23d42477e7b70258b674246463e10f975b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539532"
---
# <a name="invalidrecipient"></a>InvalidRecipient

O **elemento InvalidRecipient** contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido. 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 **InvalidRecipientType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Contém o endereço SMTP do destinatário inválido. Este elemento é obrigatório.  <br/> |
|[ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md) <br/> |Fornece um código de erro que identifica o erro específico encontrado pela solicitação. Este elemento é obrigatório.  <br/> |
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InvalidRecipients](invalidrecipients.md) <br/> |Representa os destinatários de uma solicitação de compartilhamento de pasta inválida.  <br/> |
   
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



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

