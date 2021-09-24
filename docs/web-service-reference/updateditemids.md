---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: O elemento UpdatedItemIds especifica os identificadores de itens de lembrete atualizados.
ms.openlocfilehash: 59e17e32d5df3f8a6000b05899f2fe0c5de2ec00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538608"
---
# <a name="updateditemids"></a>UpdatedItemIds

O **elemento UpdatedItemIds** especifica os identificadores de itens de lembrete atualizados. 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 **NonEmptyArrayOfItemIdsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[ItemId](itemid.md)
  
### <a name="parent-elements"></a>Elementos pai

[PerformReminderActionResponse](performreminderactionresponse.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Se a [operação PerformReminderAction](performreminderaction-operation.md) não tiver sido concluída com êxito ou nenhuma alteração tiver sido feita no servidor, o elemento **UpdatedItemIds** será retornado como um valor vazio. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[PerformReminderActionResponse](performreminderactionresponse.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

