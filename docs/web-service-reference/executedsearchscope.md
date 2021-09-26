---
title: ExecutedSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExecutedSearchScope
api_type:
- schema
ms.assetid: 2de5f0ad-43f2-4d38-b520-06540066564e
description: O elemento ExecutedSearchScope contém o escopo da pesquisa realizada para obter os resultados da pesquisa.
ms.openlocfilehash: 9b9d2d361d6a44b94d9d1e49963cfe040d97697f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545164"
---
# <a name="executedsearchscope"></a>ExecutedSearchScope

O **elemento ExecutedSearchScope** contém o escopo da pesquisa realizada para obter os resultados da pesquisa. 
  
```xml
<ExecutedSearchScope/>
```

 **String**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação FindMessageTrackingReport.](findmessagetrackingreport-operation.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto é opcional. Essas informações são usadas pelo aplicativo cliente para armazenar em cache os resultados com mais eficiência.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

