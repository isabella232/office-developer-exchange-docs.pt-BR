---
title: Ação (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: O elemento Action fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529690"
---
# <a name="action-pox"></a>Ação (POX)

O elemento **Action** fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta (POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [Ação (POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações de conta do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto indica se outra solicitação de descoberta automática é necessária para recuperar as informações de configuração do usuário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|redirectUrl  <br/> |Se esse valor for especificado, o elemento [RedirectUrl (POX)](redirecturl-pox.md) especificará a URL do servidor de acesso para cliente a ser usada na solicitação de descoberta automática subsequente. O aplicativo cliente deve parar de redirecionamento após 10 redirecionamentos.  <br/> |
|redirectAddr  <br/> |Se esse valor for especificado, o elemento [RedirectAddr (POX)](redirectaddr-pox.md) especificará o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.  <br/> |
|configurações  <br/> |Se esse valor for especificado, a resposta de descoberta automática conterá as configurações que são usadas para configurar a conta. A maioria das configurações será encontrada no elemento [Protocol (POX)](protocol-pox.md) .  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

