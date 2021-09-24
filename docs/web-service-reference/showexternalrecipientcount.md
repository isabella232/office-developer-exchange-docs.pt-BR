---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: O elemento ShowExternalRecipientCount indica se os consumidores da operação GetMailTips devem mostrar dicas de email que indicam o número de destinatários externos aos quais uma mensagem é endereçada.
ms.openlocfilehash: 30615dcb1091dff01cf13679e3e1ed68c8b25af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539097"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

O **elemento ShowExternalRecipientCount** indica se os consumidores da operação [GetMailTips](getmailtips-operation.md) devem mostrar dicas de email que indicam o número de destinatários externos aos quais uma mensagem é endereçada. 
  
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

O valor de texto desse elemento será **true** se os consumidores da operação [GetMailTips](getmailtips-operation.md) têm que mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada. O valor é **false** se os consumidores da operação [GetMailTips](getmailtips-operation.md) não têm que mostrar dicas de email que indicam o número de destinatários externos para os quais uma mensagem é endereçada. 
  
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



[Operação GetMailTips](getmailtips-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

