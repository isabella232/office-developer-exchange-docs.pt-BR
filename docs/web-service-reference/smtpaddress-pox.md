---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: O elemento SmtpAddress contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário.
ms.openlocfilehash: d257b193a3254afceaa72d396a8c2724bb3165c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546984"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

O **elemento SmtpAddress** contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de Descoberta Automática para descobrir informações de pasta pública para o usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o endereço SMTP atribuído ao armazenamento de pastas públicas configurado para o usuário. Esse endereço SMTP pode ser usado no elemento [EMailAddress (POX)](emailaddress-pox.md) de uma solicitação de Descoberta Automática para descobrir configurações de pasta pública. 
  
## <a name="remarks"></a>Comentários

O **elemento SmtpAddress** é um elemento filho necessário do **elemento PublicFolderInformation.** 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

