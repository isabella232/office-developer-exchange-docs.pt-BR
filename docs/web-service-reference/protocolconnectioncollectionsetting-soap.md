---
title: ProtocolConnectionCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 51f84364-9a5f-4ef2-ba82-f6ef7c65f7cb
description: O elemento ProtocolConnectionCollectionSetting representa uma coleção de configurações de conexão de protocolo de servidor.
ms.openlocfilehash: 8e641e8f720d5dcf6b7af8b78c1804e0d8057f09
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515254"
---
# <a name="protocolconnectioncollectionsetting-soap"></a>ProtocolConnectionCollectionSetting (SOAP)

O **elemento ProtocolConnectionCollectionSetting** representa uma coleção de configurações de conexão de protocolo de servidor. 
  
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
|[Name (SOAP)](name-soap.md) <br/> |Representa o nome de uma configuração.  <br/> |
|[ProtocolConnections (SOAP)](protocolconnections-soap.md) <br/> |Contém zero ou mais conexões de protocolo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

