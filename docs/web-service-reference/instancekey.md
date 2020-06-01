---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: O elemento InstanceKey especifica uma chave de instância para um item ou uma conversa.
ms.openlocfilehash: a6b55b9021fe63be7f678f0a1bcb24e88aeba005
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459970"
---
# <a name="instancekey"></a>InstanceKey

O elemento **InstanceKey** especifica uma chave de instância para um item ou uma conversa. 
  
```XML
<InstanceKey></InstanceKey>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **InstanceKey** é a chave de instância de um item ou uma conversa. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

