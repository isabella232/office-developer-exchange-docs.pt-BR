---
title: Response (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: O elemento Response representa a resposta a uma chamada GetDomainSettings para um domínio individual.
ms.openlocfilehash: e8f76127d5e812bc6805430544fe334eabd29ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540549"
---
# <a name="response-getdomainsettings-soap"></a>Response (GetDomainSettings) (SOAP)

O **elemento Response** representa a resposta a uma chamada **GetDomainSettings** para um domínio individual. 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contém a resposta para cada domínio solicitado em uma **solicitação GetDomainSettings.**  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Contém o código de erro associado à resposta, se aplicável.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Contém a mensagem de erro associada à resposta, se aplicável.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Retorna ao chamador as configurações de domínio.  <br/> |
   
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

