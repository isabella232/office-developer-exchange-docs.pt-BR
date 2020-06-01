---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: O elemento SmtpAddress representa o endereço SMTP (Simple Mail Transfer Protocol) de uma conta a ser usada para representação ou para um endereço de destinatário SMTP de um calendário ou solicitação de compartilhamento de contato.
ms.openlocfilehash: 915ff328cc384c1f2884e9fbea8c10c1ebc79288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466686"
---
# <a name="smtpaddress"></a>SmtpAddress

O elemento **smtpAddress** representa o endereço SMTP (Simple Mail Transfer Protocol) de uma conta a ser usada para representação ou para um endereço de destinatário SMTP de um calendário ou solicitação de compartilhamento de contato. 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta a ser representada quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Representa um destinatário inválido para uma mensagem de compartilhamento de calendário ou contato.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Representa uma coleção de destinatários aos quais será concedido acesso à pasta compartilhada.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um endereço SMTP é necessário.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

