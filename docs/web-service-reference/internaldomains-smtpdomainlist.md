---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: O elemento InternalDomains identifica a lista de domínios SMTP internos da organização.
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459963"
---
# <a name="internaldomains-smtpdomainlist"></a>InternalDomains (SmtpDomainList)

O elemento **InternalDomains** identifica a lista de domínios SMTP internos da organização. 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 **SmtpDomainList**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínio](domain.md) <br/> |Identifica um único domínio SMTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contém informações de configuração de serviço para o serviço de dicas de email.  <br/> |
|[ProtectionRulesConfiguration](protectionrulesconfiguration.md) <br/> |Contém informações de configuração de serviço para o serviço de regras de proteção.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento é obrigatório. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

