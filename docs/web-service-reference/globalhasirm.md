---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: O elemento GlobalHasIrm especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida por IRM.
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459466"
---
# <a name="globalhasirm"></a>GlobalHasIrm

O elemento **GlobalHasIrm** especifica se pelo menos uma mensagem na conversa e em todas as pastas é uma mensagem protegida por IRM. 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
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

O valor de texto do elemento **GlobalHasIrm** será **true** se pelo menos uma mensagem na conversa e em todas as pastas for uma mensagem protegida por IRM. Caso contrário, o valor será **false**.
  
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
   
## <a name="see-also"></a>Confira também



[Conversa (Conversatype)](conversation-conversationtype.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

