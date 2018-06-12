---
title: SmtpAddress POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: O elemento de SmtpAddress contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825507"
---
# <a name="smtpaddress-pox"></a>SmtpAddress POX)

O elemento de **SmtpAddress** contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o endereço SMTP atribuído ao repositório de pasta pública configurado para o usuário. Esse endereço SMTP pode ser usado no elemento [EMailAddress POX ()](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública. 
  
## <a name="remarks"></a>Coment�rios

O **SmtpAddress** é um elemento necessário filho do elemento **PublicFolderInformation** . 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

