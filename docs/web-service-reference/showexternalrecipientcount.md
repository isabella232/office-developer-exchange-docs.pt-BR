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
description: O elemento de ShowExternalRecipientCount indica se os consumidores da operação GetMailTips têm que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada.
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825491"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

O elemento de **ShowExternalRecipientCount** indica se os consumidores da [operação GetMailTips](getmailtips-operation.md) têm que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contém informações de configuração de serviço para o serviço de dicas de email.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto deste elemento é **true** se os consumidores da [operação GetMailTips](getmailtips-operation.md) tem que mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada. O valor é **false** se não tiver os consumidores da [operação GetMailTips](getmailtips-operation.md) mostrar as dicas de email que indicam o número de destinatários externos ao qual uma mensagem é endereçada. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetMailTips](getmailtips-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

