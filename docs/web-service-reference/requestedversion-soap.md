---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: O elemento RequestedVersion especifica a versão mínima do serviço que o cliente deseja que a solicitação seja processada.
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459164"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

O elemento **RequestedVersion** especifica a versão mínima do serviço que o cliente deseja que a solicitação seja processada. 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Solicitação (SOAP)](request-soap.md) <br/> |Contém as definições de configuração solicitadas e os usuários de destino.  <br/> |
|[Solicitação (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |Representa uma solicitação para obter as configurações de domínio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para o elemento **RequestedVersion** pode ser Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.
  
## <a name="remarks"></a>Comentários

Se esse elemento não estiver presente, será usada a versão mais recente do serviço.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

