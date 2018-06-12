---
title: Ação POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: O elemento Action fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752209"
---
# <a name="action-pox"></a>Ação POX)

O elemento **Action** fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [Ação POX)](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações da conta do usuário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa se outra solicitação de descoberta automática é necessária recuperar informações de configuração do usuário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|redirectUrl  <br/> |Se esse valor for especificado, o elemento [RedirectUrl POX ()](redirecturl-pox.md) especificará a URL do servidor de acesso para cliente a ser usado na solicitação de descoberta automática subsequente. O aplicativo cliente deve parar redirecionando após 10 redirecionamentos.  <br/> |
|redirectAddr  <br/> |Se esse valor for especificado, o elemento [RedirectAddr (POX)](redirectaddr-pox.md) especificará o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.  <br/> |
|configurações  <br/> |Se esse valor for especificado, a resposta da descoberta automática contém configurações que são usadas para configurar a conta. A maioria das configurações será encontrada no elemento de [Protocolo (POX)](protocol-pox.md) .  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

