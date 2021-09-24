---
title: Data (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: O elemento Data contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio.
ms.openlocfilehash: 69e15746f17febb74a0ec2f56eef0eaa1e298015
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535931"
---
# <a name="data-base64binary"></a>Data (base64Binary)

O **elemento Data** contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio. 
  
```XML
<Data/>
```

**xs:base64Binary**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Representa um único item a ser carregado em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O **elemento Data** contém os nomes de propriedades e os valores de um item exportado ou um item que será carregado em uma caixa de correio. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ExportItems](exportitems-operation.md)
- [Operação UploadItems](uploaditems-operation.md)

