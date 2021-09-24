---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: O elemento PhoneCallInformation especifica as informações de estado de uma chamada telefônica.
ms.openlocfilehash: 815e0ffac761b12969483752f5022f8580f6cc62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528323"
---
# <a name="phonecallinformation"></a>PhoneCallInformation

O **elemento PhoneCallInformation** especifica as informações de estado de uma chamada telefônica. 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 **PhoneCallInformationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PhoneCallState](phonecallstate.md) <br/> |Especifica o estado de uma chamada telefônica. Este elemento é obrigatório.  <br/> |
|[ConnectionFailureCause](connectionfailurecause.md) <br/> |Especifica a causa de uma falha de conexão. Este elemento é obrigatório.  <br/> |
|[SIPResponseText](sipresponsetext.md) <br/> |Especifica o texto de resposta SIP. Esse elemento é opcional.  <br/> |
|[SIPResponseCode](sipresponsecode.md) <br/> |Especifica o código de resposta SIP. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetPhoneCallInformationResponse](getphonecallinformationresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetPhoneCallInformation.](getphonecallinformation-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

