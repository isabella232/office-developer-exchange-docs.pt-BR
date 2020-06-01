---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: O elemento EcpUrl-tmHiding especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site.
ms.openlocfilehash: 68b949db8b8d98caddbac3b9f96c5d5e55b104b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463528"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

O elemento **EcpUrl-tmHiding** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para cancelar a inscrição do usuário a partir de uma caixa de correio de site. O valor do elemento **EcpUrl-tmHiding** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir. 
  
|**Parâmetro**|**Substituir por**|
|:-----|:-----|
| _Id_ <br/> |O endereço de email SMTP ou o nome distinto do X500 da caixa de correio do site.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **EcpUrl-tmHiding** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

