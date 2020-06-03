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
description: O elemento de dados contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526967"
---
# <a name="data-base64binary"></a>Dados (base64Binary)

O elemento de **dados** contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio. 
  
```XML
<Data/>
```

**xs: base64Binary**

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

O elemento de **dados** contém os nomes e valores de propriedade de um item exportado ou um item que será carregado em uma caixa de correio. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
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

