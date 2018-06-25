---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: O elemento MarkAsJunk Especifica a solicitação para mover um item para a pasta Lixo eletrônico e adicionar remetente à lista de remetentes bloqueados.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824350"
---
# <a name="markasjunk"></a>MarkAsJunk

O elemento **MarkAsJunk** Especifica a solicitação para mover um item para a pasta Lixo eletrônico e adicionar remetente à lista de remetentes bloqueados. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|IsJunk  <br/> |Um valor de texto de **true** para o atributo **IsJunk** indica que o remetente do email é adicionado à lista de remetentes bloqueados. Um valor **false** indica que o remetente do email é removido da lista de remetentes bloqueados, se o remetente do email já estiver na lista.  <br/> |
|MoveItem  <br/> |Um valor de **true** para o atributo **MoveItem** text indica que o item é movido para a pasta de lixo eletrônico padrão. Um valor **false** indica que o item não será movido para a pasta de lixo eletrônico padrão.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

