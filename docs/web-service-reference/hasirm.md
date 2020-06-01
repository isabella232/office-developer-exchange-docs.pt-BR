---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: O elemento HasIrm especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida por IRM.
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462777"
---
# <a name="hasirm"></a>HasIrm

O elemento **HasIrm** especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida por IRM. 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Conversa (Conversatype)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **HasIrm** é **true** se pelo menos uma mensagem na conversa e a pasta atual tem IRM. Caso contrário, o valor será **false**.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Conversa (Conversatype)](conversation-conversationtype.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

