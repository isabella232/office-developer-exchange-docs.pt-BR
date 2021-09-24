---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: O elemento TimeZoneContext é usado no header SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário para as propriedades DateTime dos objetos criados, atualizados e recuperados usando o Exchange Web Services (EWS).
ms.openlocfilehash: a628d4a094e70f1190f2cc0eda8cc4416bc37860
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515170"
---
# <a name="timezonecontext"></a>TimeZoneContext

O **elemento TimeZoneContext** é usado no header SOAP (Simple Object Access Protocol) para especificar a definição de fuso horário que deve ser usada como padrão ao atribuir o fuso horário para as propriedades DateTime dos objetos criados, atualizados e recuperados usando o Exchange Web Services (EWS). 
  
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
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Especifica os períodos e transições que definem um fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

