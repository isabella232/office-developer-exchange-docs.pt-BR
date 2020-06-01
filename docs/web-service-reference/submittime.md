---
title: Enviartime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: O elemento Submittime representa a hora em que a mensagem foi enviada para o servidor.
ms.openlocfilehash: e4409d962988ee308e0c0b461f9448ef68067fe8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467050"
---
# <a name="submittime"></a>Enviartime

O elemento **submittime** representa a hora em que a mensagem foi enviada para o servidor. 
  
```XML
<SubmitTime/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma data/hora será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

