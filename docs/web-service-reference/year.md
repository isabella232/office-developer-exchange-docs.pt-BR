---
title: Ano
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: O elemento Year é usado para definir um fuso horário que muda dependendo do ano. Esse elemento é opcional. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 80b4ce642a7a08631140e583fb9d92143f485ea3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509277"
---
# <a name="year"></a>Ano

O **elemento Year** é usado para definir um fuso horário que muda dependendo do ano. Esse elemento é opcional. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<Year/>
```

**cadeia de caracteres**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> |Representa um deslocamento do tempo em relação ao TEMPO Universal Coordenado (UTC) representado pelo elemento [Bias (UTC).](bias-utc.md)  <br/> |
|[DaylightTime](daylighttime.md) <br/> |Representa um deslocamento do tempo em relação ao UTC (Tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O elemento Year aceita uma cadeia de caracteres que representa um ano. O formato de ano é YYYY.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

