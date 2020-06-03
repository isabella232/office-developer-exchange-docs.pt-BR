---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: O elemento ShowExternalRecipientCount indica se os consumidores da operação GetQuery devem mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460467"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

O elemento **ShowExternalRecipientCount** indica se os consumidores da [operação](getmailtips-operation.md) GetQuery devem mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
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

O valor de texto desse elemento será **true** se os consumidores da [operação](getmailtips-operation.md) GetQuery precisarem Mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada. O valor é **false** se os consumidores da [operação](getmailtips-operation.md) GetQuery não precisam mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação](getmailtips-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

