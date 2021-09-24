---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: O elemento RecurringMasterItemIdRanges especifica uma matriz de intervalos de ocorrência.
ms.openlocfilehash: 582cbe27d468c1ff7ec22f03ba9f6976d244e234
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529367"
---
# <a name="recurringmasteritemidranges"></a>RecurringMasterItemIdRanges

O **elemento RecurringMasterItemIdRanges** especifica uma matriz de intervalos de ocorrência. 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 **RecurringMasterItemIdRangesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |O valor de texto do **atributo Id** é o identificador exclusivo de um item mestre recorrente. Este é um **valor de cadeia de** caracteres.  <br/> |
|**ChangeKey** <br/> |O valor de texto do **atributo ChangeKey** é a chave de alteração do item mestre recorrente. Este é um **valor de cadeia de** caracteres.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[Ranges](ranges.md)
  
### <a name="parent-elements"></a>Elementos pai

[ItemIds](itemids.md)  |  [GlobalItemIds](globalitemids.md)  |  [DraftItemIds](draftitemids.md)  |  [ContactIds](contactids.md)  |  [GroupIds](groupids.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

