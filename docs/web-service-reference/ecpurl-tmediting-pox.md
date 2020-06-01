---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: O elemento EcpUrl-tmEditing especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente.
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463535"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

O elemento **EcpUrl-tmEditing** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
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

O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para editar uma caixa de correio de site existente. O valor do elemento **EcpUrl-tmEditing** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir. 
  
|**Parâmetro**|**Substituir por**|
|:-----|:-----|
| _Id_ <br/> |O endereço de email SMTP ou o nome distinto do X500 da caixa de correio do site.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **EcpUrl-tmEditing** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

