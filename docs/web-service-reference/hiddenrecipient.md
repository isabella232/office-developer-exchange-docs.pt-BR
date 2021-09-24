---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: O elemento HiddenRecipient indica que o destinatário foi adicionado por uma política de organização que deve ser ocultada de usuários nãoprivilegados.
ms.openlocfilehash: 24d7dcad5b8b744351804160ef8d9988b9e393a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539686"
---
# <a name="hiddenrecipient"></a>HiddenRecipient

O **elemento HiddenRecipient** indica que o destinatário foi adicionado por uma política de organização que deve ser ocultada de usuários nãoprivilegados. 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações de um único evento para um destinatário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **verdadeiro ou** **falso.** Um valor **verdadeiro** indica que o usuário foi adicionado por uma política de organização; um valor **false** indica que o usuário não foi adicionado por uma política de organização. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

