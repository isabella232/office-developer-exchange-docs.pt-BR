---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: O elemento DomainSettingsErrors contém informações de erro para configurações que não puderam ser retornadas.
ms.openlocfilehash: d34fa8be4b4bc24e99fb6b1cd36d02e4c4915dd7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544210"
---
# <a name="domainsettingerrors-soap"></a>DomainSettingErrors (SOAP)

O **elemento DomainSettingsErrors** contém informações de erro para configurações que não puderam ser retornadas. 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 **DomainSettingsErrors**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainSettingError (SOAP)](domainsettingerror-soap.md) <br/> |Representa um erro que ocorreu durante a recuperação de uma configuração de domínio. Isso representa um erro de uma [solicitação de operação GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contém as configurações solicitadas para o domínio especificado.  <br/> |
   
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

