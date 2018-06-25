---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: O elemento EwsPartnerUrl Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email.
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752124"
---
# <a name="ewspartnerurl-pox"></a>EwsPartnerUrl (POX)

O elemento **EwsPartnerUrl** Especifica a URL da instância do ponto de extremidade recomendada para o Exchange Web Services (EWS) para um usuário habilitado para email. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[EwsPartnerUrl (POX)](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a URL do ponto de extremidade EWS para o usuário.
  
## <a name="remarks"></a>Comentários

O **EwsPartnerUrl** é um elemento filho opcionais do elemento de **protocolo** . É equivalente ao elemento [EwsUrl POX ()](ewsurl-pox.md) . 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

