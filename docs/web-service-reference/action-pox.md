---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: O elemento Action fornece informações que são usadas para determinar se outra solicitação de Descoberta Automática é necessária para retornar as informações de configuração do usuário.
ms.openlocfilehash: b1c07fefc6b8033b9b93bd044c04fb07ba289177
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513854"
---
# <a name="action-pox"></a>Action (POX)

O **elemento Action** fornece informações que são usadas para determinar se outra solicitação de Descoberta Automática é necessária para retornar as informações de configuração do usuário. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Action (POX)](action-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |Especifica as configurações da conta para o usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa se outra solicitação de Descoberta Automática é necessária para recuperar as informações de configuração do usuário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|redirectUrl  <br/> |Se esse valor for especificado, o [elemento RedirectUrl (POX)](redirecturl-pox.md) especificará a URL do servidor de Acesso para Cliente a ser usada na solicitação de Descoberta Automática subsequente. O aplicativo cliente deve parar de redirecionar após 10 redirecionamentos.  <br/> |
|redirectAddr  <br/> |Se esse valor for especificado, o [elemento RedirectAddr (POX)](redirectaddr-pox.md) especificará o endereço de email que deve ser usado para uma solicitação de Descoberta Automática subsequente.  <br/> |
|configurações  <br/> |Se esse valor for especificado, a resposta descoberta automática conterá configurações usadas para configurar a conta. A maioria das configurações será encontrada no elemento [Protocolo (POX).](protocol-pox.md)  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

