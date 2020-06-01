---
title: EcpUrl-MT (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: O elemento EcpUrl-MT especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações de controle de mensagens de email de um usuário habilitado para email.
ms.openlocfilehash: 097811add5635bca14c659814652bca244a1398d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458709"
---
# <a name="ecpurl-mt-pox"></a>EcpUrl-MT (POX)

O elemento **EcpUrl-MT** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de controle de mensagens de email de um usuário habilitado para email. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-MT (POX)](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
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

O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de controle de email do usuário. O valor do elemento **EcpUrl-MT** contém parâmetros contidos nos caracteres ' < ' e ' > ' que são substituídos pelo cliente, conforme mostrado na tabela a seguir. 
  
|**Parâmetro**|**Substituir por**|
|:-----|:-----|
| _IsOwa_ <br/> |n  <br/> |
| _MsgID_ <br/> |Identificador de mensagem da Internet da mensagem a ser rastreada conforme especificado pelo cabeçalho Message-ID.  <br/> |
| _MBX_ <br/> |O endereço SMTP do proprietário da caixa de correio.  <br/> |
| _Sender_ <br/> |O endereço SMTP do remetente da mensagem.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **EcpUrl-MT** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

