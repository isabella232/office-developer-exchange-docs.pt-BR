---
title: Dados (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: O elemento de dados contém os dados de um item para carregar em uma caixa de correio ou de um único item exportado.
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751670"
---
# <a name="data-base64binary"></a>Dados (base64Binary)

O elemento de **dados** contém os dados de um item para carregar em uma caixa de correio ou de um único item exportado. 
  
```XML
<Data/>
```

**base64Binary**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para exportar um item de caixa de correio única.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Representa um único item para carregar em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

O elemento de **dados** contém os nomes de propriedade e valores para um item que será carregado em uma caixa de correio ou de um item exportado. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ExportItems](exportitems-operation.md)
- [Operação UploadItems](uploaditems-operation.md)

