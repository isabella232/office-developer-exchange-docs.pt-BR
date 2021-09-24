---
title: LargeAudienceThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- LargeAudienceThreshold
api_type:
- schema
ms.assetid: dacd9db7-b8f0-445d-a3d1-3356b8c2bcd1
description: O elemento LargeAudienceThreshold representa o limite de audiência grande para um cliente.
ms.openlocfilehash: c342fa63b19d5af52fe49362ae46b9848addaa0b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540857"
---
# <a name="largeaudiencethreshold"></a>LargeAudienceThreshold

O **elemento LargeAudienceThreshold** representa o limite de audiência grande para um cliente. 
  
```XML
<LargeAudienceThreshold/>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contém informações de configuração de serviço para o serviço de dicas de email.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é um número inteiro que representa o limite de audiência que indica que a mensagem irá para mais de uma pessoa.
  
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



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

