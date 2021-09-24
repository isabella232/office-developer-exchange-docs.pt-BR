---
title: Flag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: O elemento Flag especifica um sinalizador em um item de caixa de correio.
ms.openlocfilehash: dffc550dc4235c2121b6641f3a6eac30594f75b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513693"
---
# <a name="flag"></a>Flag

O **elemento Flag** especifica um sinalizador em um item de caixa de correio. 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **FlagType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |Contém o status do sinalizador agregado para itens na pasta atual.  <br/> |
|[StartDate](startdate.md) <br/> |Representa a data de início de um item.  <br/> |
|[DueDate](duedate.md) <br/> |Representa a data em que um item é devido.  <br/> |
|[CompleteDate](completedate.md) <br/> |Representa a data em que um item foi concluído.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

