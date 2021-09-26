---
title: SubmittedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubmittedTime
api_type:
- schema
ms.assetid: 45c8fa36-c539-42ca-99dc-1ac33cc54afc
description: O elemento SubmittedTime representa a hora em que a mensagem entrou no servidor.
ms.openlocfilehash: 68df76b7ace8c8d665eff87c995a2b658be7e61c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545850"
---
# <a name="submittedtime"></a>SubmittedTime

O **elemento SubmittedTime** representa a hora em que a mensagem entrou no servidor. 
  
```XML
<SubmittedTime/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contém um único resultado de mensagem para [um elemento FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

 Um valor de texto que representa uma data/hora é necessário se esse elemento for usado. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

