---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: O elemento SmtpAddress contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário.
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468639"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

O elemento **smtpAddress** contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta (POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o endereço SMTP atribuído ao armazenamento de pasta pública configurado para o usuário. Esse endereço SMTP pode ser usado no elemento de [EMailAddress (POX)](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública. 
  
## <a name="remarks"></a>Comentários

O elemento **smtpAddress** é um elemento filho obrigatório do elemento **PublicFolderInformation** . 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

