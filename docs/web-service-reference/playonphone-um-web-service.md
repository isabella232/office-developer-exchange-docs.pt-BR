---
title: PlayOnPhone (serviço Web da UM)
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
description: O elemento PlayOnPhone define uma solicitação para reproduzir um item em um telefone.
ms.openlocfilehash: 9acbf9edbf4a889506558b24f5736a44d5015d3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44434075"
---
# <a name="playonphone-um-web-service"></a>PlayOnPhone (serviço Web da UM)

O elemento **PlayOnPhone** define uma solicitação para reproduzir um item em um telefone. 
  
[PlayOnPhone (serviço Web da UM)](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 **complexType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EntryID (serviço Web da UM)](entryid-um-web-service.md) <br/> |Contém o valor que representa o identificador do item a ser tocado no telefone em uma solicitação de [operação do PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) .  <br/> |
|[dialstring (serviço Web da UM)](dialstring-um-web-service.md) <br/> |Contém o valor do número de telefone a ser discado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação PlayOnPhone (serviço Web da UM)](playonphone-operation-um-web-service.md)

