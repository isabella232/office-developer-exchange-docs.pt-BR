---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: O elemento RecurringMasterItemId (ItemIdType) identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados.
ms.openlocfilehash: 491bb6686ad6cc9ee8169144b659d828e3920e45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522737"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

O **elemento RecurringMasterItemId (ItemIdType)** identifica um item mestre de recorrência identificando os identificadores de um de seus itens de ocorrência relacionados. 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

****

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Identifica uma única ocorrência de um item mestre recorrente. Esse atributo é necessário.  <br/> |
|ChangeKey  <br/> |Identifica uma versão específica de uma única ocorrência de um item mestre recorrente. Além disso, o item mestre recorrente também é identificado porque ele e a única ocorrência conterão a mesma chave de alteração. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Lembrete](reminder.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Lembrete](reminder.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

