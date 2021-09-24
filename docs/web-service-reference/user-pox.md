---
title: User (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: O elemento User fornece informações específicas do usuário.
ms.openlocfilehash: 832e0a63e75a08406b3aa397ac29ad5aa300cfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522400"
---
# <a name="user-pox"></a>User (POX)

O **elemento User** fornece informações específicas do usuário. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[User (POX)](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Representa o nome para exibição do usuário.  <br/> |
|[LegacyDN (POX)](legacydn-pox.md) <br/> |Identifica a caixa de correio de um usuário pelo nome diferenciado herdado.  <br/> |
|[DeploymentId (POX)](deploymentid-pox.md) <br/> |Identifica exclusivamente a floresta Exchange.  <br/> |
|[AutoDiscoverSMTPAddress (POX)](autodiscoversmtpaddress-pox.md) <br/> |Contém o endereço SMTP do usuário que é usado para o processo de Descoberta Automática.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Contém a resposta do serviço descoberta automática.  <br/> |
   
## <a name="remarks"></a>Comentários

As solicitações e respostas de descoberta automática devem ser codificadas utf-8.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

