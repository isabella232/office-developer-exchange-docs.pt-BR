---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: O elemento PublicFolderInformation contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824927"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

O elemento **PublicFolderInformation** contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SmtpAddress POX)](smtpaddress-pox.md) <br/> |Contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário. Esse endereço SMTP pode ser usado no elemento [EMailAddress POX ()](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações da conta do usuário.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O **PublicFolderInformation** é um elemento filho opcionais do elemento de **conta** . 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

