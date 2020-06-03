---
title: Erro (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: O elemento error contém uma resposta de erro de descoberta automática.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530646"
---
# <a name="error-pox"></a>Erro (POX)

O elemento **Error** contém uma resposta de erro de descoberta automática. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Erro (POX)](error-pox.md)
  
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
|Hora  <br/> |Representa a hora em que a resposta de erro foi retornada.  <br/> |
|Id  <br/> |Representa um hash do nome do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |Contém o código de erro para uma resposta de descoberta automática de erro.  <br/> |
|[Mensagem (POX)](message-pox.md) <br/> |Contém a mensagem de erro para uma resposta de descoberta automática de erro.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contém os dados de depuração de uma resposta de descoberta automática de erro.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Contém uma resposta de erro de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

