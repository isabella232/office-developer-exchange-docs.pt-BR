---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: O elemento TimeZoneContext é usado no cabeçalho SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário das propriedades DateTime dos objetos criados, atualizados e recuperados usando o EWS (serviços Web do Exchange).
ms.openlocfilehash: 26727317ccf34338e8d62ec92bd7a44d43a6cfdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460250"
---
# <a name="timezonecontext"></a>TimeZoneContext

O elemento **TimeZoneContext** é usado no cabeçalho SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário das propriedades DateTime dos objetos criados, atualizados e recuperados usando o EWS (serviços Web do Exchange). 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 **TimeZoneContextType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Especifica os períodos e as transições que definem um fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

