---
title: Error (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: O elemento Error contém uma resposta de erro de Descoberta Automática.
ms.openlocfilehash: 2f96f8b9d6d154aac6f10924095b5a5864e76750
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530886"
---
# <a name="error-pox"></a>Error (POX)

O **elemento Error** contém uma resposta de erro de Descoberta Automática. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Error (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Time  <br/> |Representa a hora em que a resposta de erro foi retornada.  <br/> |
|Id  <br/> |Representa um hash do nome do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Contém o código de erro para uma resposta de Descoberta Automática de erro.  <br/> |
|[Message (POX)](message-pox.md) <br/> |Contém a mensagem de erro para uma resposta de Descoberta Automática de erro.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contém os dados de depuração para uma resposta de Descoberta Automática de erro.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Contém uma resposta de erro de Descoberta Automática.  <br/> |
   
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

