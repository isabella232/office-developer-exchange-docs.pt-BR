---
title: PlayOnPhone (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: O elemento PlayOnPhone define uma solicitação para reproduzir um item em um telefone.
ms.openlocfilehash: 240c8f474c87e0c123a6d8239eb691079385e348
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527986"
---
# <a name="playonphone-um-web-service"></a>PlayOnPhone (serviço Web de Unificação de Mensagens)

O **elemento PlayOnPhone** define uma solicitação para reproduzir um item em um telefone. 
  
[PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-um-web-service.md)
  
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
|[entryId (serviço Web de Unificação de Mensagens)](entryid-um-web-service.md) <br/> |Contém o valor que representa o identificador do item a ser reproduzir no telefone em uma solicitação de operação [do PlayOnPhone (serviço Web](playonphone-operation-um-web-service.md) da UM).  <br/> |
|[dialString (serviço Web de Unificação de Mensagens)](dialstring-um-web-service.md) <br/> |Contém o valor para o número de telefone discar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-operation-um-web-service.md)

