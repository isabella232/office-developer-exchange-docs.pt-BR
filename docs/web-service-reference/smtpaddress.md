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
description: O elemento SmtpAddress representa o endereço de Simple Mail Transfer Protocol (SMTP) de uma conta a ser usada para representação ou um endereço de destinatário de Simple Mail Transfer Protocol (SMTP) de um calendário ou uma solicitação de compartilhamento do contato.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825511"
---
# <a name="smtpaddress"></a>SmtpAddress

O elemento **SmtpAddress** representa o endereço de Simple Mail Transfer Protocol (SMTP) de uma conta a ser usada para representação ou um endereço de destinatário de Simple Mail Transfer Protocol (SMTP) de um calendário ou uma solicitação de compartilhamento do contato. 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Representa um destinatário inválido para um compartilhamento de calendário ou mensagem de compartilhamento do contato.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Representa uma coleção dos destinatários que receberão acesso à pasta compartilhada.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um endereço SMTP.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

