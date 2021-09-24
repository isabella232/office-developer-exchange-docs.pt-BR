---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: O elemento DomainResponses contém uma matriz de respostas para as configurações de cada domínio solicitado.
ms.openlocfilehash: 307cae0aca0f34b0a33edd41248f8f572f2a80af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540107"
---
# <a name="domainresponses-soap"></a>DomainResponses (SOAP)

O **elemento DomainResponses** contém uma matriz de respostas para as configurações de cada domínio solicitado. 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 **ArrayOfDomainResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Representa a resposta a uma solicitação de operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio e retorna as configurações de domínio.  <br/> |
|[Response (GetDomainSettings) (SOAP)](response-getdomainsettingssoap.md) <br/> |Representa a resposta a [uma chamada da operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.  <br/> |
   
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

- [Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

