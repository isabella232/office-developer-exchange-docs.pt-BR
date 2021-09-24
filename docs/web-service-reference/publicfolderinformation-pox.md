---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: O elemento PublicFolderInformation contém informações que os clientes podem usar para enviar uma solicitação de Descoberta Automática para descobrir informações de pasta pública para o usuário.
ms.openlocfilehash: d77ea350f05c5d6137d3b67cfd49119bf9590e53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540619"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

O **elemento PublicFolderInformation** contém informações que os clientes podem usar para enviar uma solicitação de Descoberta Automática para descobrir informações de pasta pública para o usuário. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário. Esse endereço SMTP pode ser usado no elemento [EMailAddress (POX)](emailaddress-pox.md) de uma solicitação de Descoberta Automática para descobrir configurações de pasta pública.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Especifica as configurações da conta para o usuário.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento PublicFolderInformation** é um elemento filho opcional do **elemento** Account. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

