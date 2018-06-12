---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: O elemento RecurringMasterItemId (ItemIdType) identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825010"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

O elemento **RecurringMasterItemId (ItemIdType)** identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência. 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

****

|**Attribute**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Identifica uma única ocorrência de um item mestre recorrente. Este atributo é necessário.  <br/> |
|ChangeKey  <br/> |Identifica uma versão específica de uma única ocorrência de um item mestre recorrente. Além disso, o item mestre recorrente também é identificado porque ele e a ocorrência única irá conter a mesma chave de alteração. Este atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Lembrete](reminder.md)
  
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



[Lembrete](reminder.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

