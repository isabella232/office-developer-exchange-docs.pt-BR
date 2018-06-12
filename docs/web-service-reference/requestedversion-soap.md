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
description: O elemento RequestedVersion Especifica a versão mínima do serviço que o cliente quer a solicitação a serem processados em.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825134"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

O elemento **RequestedVersion** Especifica a versão mínima do serviço que o cliente quer a solicitação a serem processados em. 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Solicitação (SOAP)](request-soap.md) <br/> |Contém as definições de configuração solicitado e os usuários de destino.  <br/> |
|[Solicitação (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |Representa uma solicitação para obter as configurações de domínio.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto para o elemento **RequestedVersion** pode ser Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.
  
## <a name="remarks"></a>Coment�rios

Se esse elemento não estiver presente, a versão mais recente do serviço é usada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

