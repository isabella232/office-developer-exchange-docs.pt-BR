---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: O elemento PhoneCallId especifica o identificador de uma chamada telefônica. Este elemento é obrigatório.
ms.openlocfilehash: 00b23c8b4023a6fef9c27295c8e023e5324b7026
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528316"
---
# <a name="phonecallid"></a>PhoneCallId

O **elemento PhoneCallId** especifica o identificador de uma chamada telefônica. Este elemento é obrigatório. 
  
```xml
<PhoneCallId Id="" />
```

 **PhoneCallIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Identifica a chamada telefônica para desconectar. Esse atributo é necessário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DisconnectPhoneCall](disconnectphonecall.md) <br/> |Representa uma solicitação para desconectar uma chamada.  <br/> |
|[GetPhoneCallInformation](getphonecallinformation.md) <br/> |Representa uma solicitação para obter informações de chamada telefônica.  <br/> |
|[PlayOnPhoneResponse (Exchange Web Services)](playonphoneresponse-exchange-web-services.md) <br/> |Define uma resposta a uma solicitação PlayOnPhone.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

