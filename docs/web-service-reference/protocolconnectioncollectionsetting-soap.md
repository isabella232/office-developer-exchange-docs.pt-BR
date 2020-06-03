---
title: ProtocolConnectionCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 51f84364-9a5f-4ef2-ba82-f6ef7c65f7cb
description: O elemento ProtocolConnectionCollectionSetting representa uma coleção de configurações de conexão de protocolo do servidor.
ms.openlocfilehash: 59e082138b8a40d201791653103c79160765f2fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462392"
---
# <a name="protocolconnectioncollectionsetting-soap"></a>ProtocolConnectionCollectionSetting (SOAP)

O elemento **ProtocolConnectionCollectionSetting** representa uma coleção de configurações de conexão de protocolo do servidor. 
  
```XML
<ProtocolConnectionCollectionSetting/>
   <Name/>
   <ProtocolConnections/>
</ProtocolConnectionCollectionSetting>
```

 **ProtocolConnectionCollectionSetting**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (SOAP)](name-soap.md) <br/> |Representa o nome de uma configuração.  <br/> |
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |Contém zero ou mais conexões de protocolo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

