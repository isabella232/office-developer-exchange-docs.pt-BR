---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: O elemento ProtocolConnection representa a conexão de protocolo do cliente Web do servidor.
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528857"
---
# <a name="protocolconnection-soap"></a>ProtocolConnection (SOAP)

O elemento **ProtocolConnection** representa a conexão de protocolo do cliente Web do servidor. 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 **ProtocolConnection**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome do host (SOAP)](hostname-soap.md) <br/> |Representa a parte do nome do host do nome completo do computador.  <br/> |
|[Porta (SOAP)](port-soap.md) <br/> |Representa o número da porta a ser usado para o protocolo.  <br/> |
|[EncryptionMethod (SOAP)](encryptionmethod-soap.md) <br/> |Representa o método criptográfico que é usado para os protocolos POP, IMAP e SMTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |Contém zero ou mais conexões de protocolo.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[ProtocolConnectionCollectionSetting (SOAP)](protocolconnectioncollectionsetting-soap.md)

