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
description: O elemento de erro contém uma resposta de erro de descoberta automática.
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752086"
---
# <a name="error-pox"></a>Erro (POX)

O elemento de **erro** contém uma resposta de erro de descoberta automática. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Erro (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Hora  <br/> |Representa a hora em que a resposta de erro foi retornada.  <br/> |
|Id  <br/> |Representa um hash do nome do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode POX)](errorcode-pox.md) <br/> |Contém o código de erro para um erro de resposta de descoberta automática.  <br/> |
|[Mensagem (POX)](message-pox.md) <br/> |Contém a mensagem de erro para um erro de resposta de descoberta automática.  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |Contém os dados de depuração para um erro de resposta de descoberta automática.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Contém uma resposta de erro de descoberta automática.  <br/> |
   
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

