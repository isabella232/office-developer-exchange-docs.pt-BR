---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: O elemento MarkAsJunk especifica a solicitação para mover um item para a pasta de lixo eletrônico e para adicionar o remetente à lista de remetentes bloqueados.
ms.openlocfilehash: 252c36b8bb3662ffd6c0fe470a81b6f0b55acb69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544084"
---
# <a name="markasjunk"></a>MarkAsJunk

O **elemento MarkAsJunk** especifica a solicitação para mover um item para a pasta de lixo eletrônico e para adicionar o remetente à lista de remetentes bloqueados. 
  
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
|IsJunk  <br/> |Um valor de texto **true para** o **atributo IsJunk** indica que o remetente de email é adicionado à lista de remetentes bloqueados. Um valor **false** indica que o remetente de email é removido da lista de remetentes bloqueados, se o remetente de email já estiver na lista.  <br/> |
|MoveItem  <br/> |Um valor de texto **true para** o **atributo MoveItem** indica que o item é movido para a pasta de lixo eletrônico padrão. Um valor **false** indica que o item não é movido para a pasta de lixo eletrônico padrão.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

