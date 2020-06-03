---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: O elemento MarkAsJunk especifica a solicitação para mover um item para a pasta lixo eletrônico e adicionar o remetente à lista de remetentes bloqueados.
ms.openlocfilehash: 99adc423864f3096772394ef290df20e158e457d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467078"
---
# <a name="markasjunk"></a>MarkAsJunk

O elemento **MarkAsJunk** especifica a solicitação para mover um item para a pasta lixo eletrônico e adicionar o remetente à lista de remetentes bloqueados. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Islixo eletrônico  <br/> |Um valor de texto **true** para o atributo **isjunk** indica que o remetente de email é adicionado à lista de remetentes bloqueados. Um valor **false** indica que o remetente de email será removido da lista de remetentes bloqueados, se o remetente de email já estiver na lista.  <br/> |
|MoveItem  <br/> |Um valor de texto **true** para o atributo **MoveItem** indica que o item é movido para a pasta de lixo eletrônico padrão. Um valor **false** indica que o item não é movido para a pasta de lixo eletrônico padrão.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

