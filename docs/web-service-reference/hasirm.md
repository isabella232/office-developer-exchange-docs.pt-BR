---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: O elemento HasIrm Especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida do IRM.
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823803"
---
# <a name="hasirm"></a>HasIrm

O elemento **HasIrm** Especifica se pelo menos uma mensagem na conversa e a pasta atual é uma mensagem protegida do IRM. 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Conversa (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **HasIrm** é **true** se pelo menos uma mensagem na conversa e a pasta atual tiver IRM. Caso contrário, o valor é **false**.
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Conversa (ConversationType)](conversation-conversationtype.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

