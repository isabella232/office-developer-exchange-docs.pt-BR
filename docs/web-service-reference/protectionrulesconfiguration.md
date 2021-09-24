---
title: ProtectionRulesConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: O elemento ProtectionRulesConfiguration contém informações de configuração de serviço para o serviço de regras de proteção.
ms.openlocfilehash: 0d88f5c8ef414c96ae5f65cf3f82362fe2137472
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516401"
---
# <a name="protectionrulesconfiguration"></a>ProtectionRulesConfiguration

O **elemento ProtectionRulesConfiguration** contém informações de configuração de serviço para o serviço de regras de proteção. 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 **ProtectionRulesServiceConfiguration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**RefreshInterval** <br/> |Especifica com que frequência, em horas inteiras, o cliente deve solicitar regras de proteção do servidor. Esse atributo é necessário e seu valor deve ser um inteiro igual ou maior que 1.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regras ](rules-ex15websvcsotherref.md) <br/> |Uma matriz de regras de proteção. Este elemento é obrigatório.  <br/> |
|[InternalDomains (SmtpDomainList)](internaldomains-smtpdomainlist.md) <br/> |Identifica a lista de domínios SMTP internos da organização. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém configurações de serviço.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

A configuração do serviço de regras de proteção é composta por uma lista de regras, domínios internos e um intervalo de atualização.
  
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

