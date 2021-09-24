---
title: StartDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartDateTime
api_type:
- schema
ms.assetid: 6fd41b7b-6c83-43b6-8b16-0bdb3d173d73
description: O elemento StartDateTime especifica a data e a hora de início de uma regra ou uma pesquisa.
ms.openlocfilehash: 524858a0b33a25defeae339f7780a7b47c4f21cf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517697"
---
# <a name="startdatetime"></a>StartDateTime

O **elemento StartDateTime** especifica a data e a hora de início de uma regra ou uma pesquisa. 
  
```XML
<StartDate/>
```

**dateTime**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Especifica critérios para os tipos de mensagens a encontrar.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Especifica o intervalo de datas no qual as mensagens de entrada têm que ser recebidas para que a condição ou exceção seja aplicada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

 Um valor de texto que representa uma data/hora é necessário se esse elemento for usado. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

