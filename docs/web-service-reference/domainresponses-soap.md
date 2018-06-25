---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: O elemento DomainResponses contém uma matriz de respostas para as configurações do cada domínio solicitada.
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751923"
---
# <a name="domainresponses-soap"></a>DomainResponses (SOAP)

O elemento **DomainResponses** contém uma matriz de respostas para as configurações do cada domínio solicitada. 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 **ArrayOfDomainResponse**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Representa a resposta a uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio e retorna as configurações de domínio.  <br/> |
|[Resposta (GetDomainSettings) (SOAP)](response-getdomainsettingssoap.md) <br/> |Representa a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

