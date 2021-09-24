---
title: Internal (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: O elemento Interno contém a coleção de URLs que um cliente pode usar para se conectar Exchange de dentro da rede da organização.
ms.openlocfilehash: f87c5e21eff87965c9b6ff6f3d59e2b3a37b87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541116"
---
# <a name="internal-pox"></a>Internal (POX)

O **elemento Internal** contém a coleção de URLs que um cliente pode usar para se conectar Exchange de dentro da rede da organização. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OWAUrl (POX)](owaurl-pox.md) <br/> |Descreve a URL e o esquema de autenticação que é usado para acessar um computador específico que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada que hospeda o Outlook Web Access.  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada. Este **elemento Protocol** tem apenas dois elementos filho: um elemento Type [(POX)](type-pox.md) que especifica o protocolo de conexão e um [elemento ASUrl (POX),](asurl-pox.md) especificando o ponto de extremidade EWS para o serviço Web de disponibilidade.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento Internal** é um elemento filho opcional do elemento **Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

