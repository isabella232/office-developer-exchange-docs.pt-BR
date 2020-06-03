---
title: EncryptionMethod (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bc632c85-ec74-4a00-baec-df5973e032fa
description: O elemento EncryptionMethod representa o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.
ms.openlocfilehash: 26236d9b08eae1bcabfd9aac59f5b01714ba9841
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530653"
---
# <a name="encryptionmethod-soap"></a>EncryptionMethod (SOAP)

O elemento **EncryptionMethod** representa o método criptográfico que é usado para os protocolos pop, IMAP e SMTP. 
  
```XML
<EncryptionMethod/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ProtocolConnection (SOAP)](protocolconnection-soap.md) <br/> |Representa a conexão de protocolo do cliente Web do servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)

