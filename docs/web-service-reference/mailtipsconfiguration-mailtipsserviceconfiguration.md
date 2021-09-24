---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: O elemento MailTipsConfiguration contém informações de configuração de serviço para o serviço de dicas de email.
ms.openlocfilehash: eb86291572f6854710d01badcee2db24406844c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524032"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a>MailTipsConfiguration (MailTipsServiceConfiguration)

O **elemento MailTipsConfiguration** contém informações de configuração de serviço para o serviço de dicas de email. 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 **MailTipsServiceConfiguration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsEnabled](mailtipsenabled.md) <br/> |Indica se o serviço de dicas de email está disponível. Este elemento é obrigatório.  <br/> |
|[MaxRecipientsPerGetMailTipsRequest](maxrecipientspergetmailtipsrequest.md) <br/> |Indica o número máximo de destinatários que podem ser passados para a [operação GetMailTips](getmailtips-operation.md). Este elemento é obrigatório.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Representa o tamanho máximo de mensagem que um destinatário pode aceitar. Este elemento é obrigatório.  <br/> |
|[LargeAudienceThreshold](largeaudiencethreshold.md) <br/> |Representa o limite de audiência grande para um cliente. Este elemento é obrigatório.  <br/> |
|[ShowExternalRecipientCount](showexternalrecipientcount.md) <br/> |Indica se os consumidores da operação [GetMailTips](getmailtips-operation.md) devem mostrar dicas de email que indicam o número de destinatários externos aos quais uma mensagem é endereçada. Este elemento é obrigatório.  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |Identifica a lista de domínios SMTP internos da organização. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém configurações de serviço.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
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

