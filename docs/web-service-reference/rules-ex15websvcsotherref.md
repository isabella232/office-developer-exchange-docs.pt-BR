---
title: Regras
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: O elemento de regras contém uma matriz de regras de proteção.
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825269"
---
# <a name="rules"></a>Regras

O elemento de **regras** contém uma matriz de regras de proteção. 
  
```xml
<Rules>   <Rule/></Rules>
```

 **ArrayOfProtectionRulesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule](rule.md) <br/> |Contém uma regra de proteção do único. Esse elemento pode ocorrer zero ou mais vezes. Esse elemento ocorre zero vezes quando não há regras de proteção são definidas pela organização. Uma ou mais vezes ocorre se não houver pelo menos uma regra definida pela organização.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ProtectionRulesConfiguration](protectionrulesconfiguration.md) <br/> |Contém a configuração do serviço para o serviço de regras de proteção.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

