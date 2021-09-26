---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: O elemento GetDomainSettingsRequest representa uma solicitação de operação getDomainSettings (SOAP).
ms.openlocfilehash: 4c222c6832b5be7da598de3390d13123749f8b0f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544989"
---
# <a name="getdomainsettingsrequest-soap"></a>GetDomainSettingsRequest (SOAP)

O **elemento GetDomainSettingsRequest** representa uma solicitação de operação [getDomainSettings (SOAP).](getdomainsettings-operation-soap.md) 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |Representa uma coleção de identificadores de domínio.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das configurações de domínio solicitadas.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Especifica a versão do servidor que o provedor usará.  <br/> |
   
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



[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

