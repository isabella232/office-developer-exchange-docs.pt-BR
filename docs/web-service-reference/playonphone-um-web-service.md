---
title: PlayOnPhone (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: O elemento de PlayOnPhone define uma solicitação para tocar um item em um telefone.
ms.openlocfilehash: 7e5c1e25512a59d1ac3295b476fcc2b6b0f5a2b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824825"
---
# <a name="playonphone-um-web-service"></a>PlayOnPhone (serviço web de Unificação de mensagens)

O elemento de **PlayOnPhone** define uma solicitação para tocar um item em um telefone. 
  
[PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[entryId (serviço web de Unificação de mensagens)](entryid-um-web-service.md) <br/> |Contém o valor que representa o identificador do item para tocar no telefone em uma solicitação de [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) .  <br/> |
|[dialString (serviço web de Unificação de mensagens)](dialstring-um-web-service.md) <br/> |Contém o valor para o número de telefone discar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md)

