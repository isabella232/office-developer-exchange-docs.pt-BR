---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: O elemento IsUndecidedApprovalRequest especifica se uma mensagem de solicitação de aprovação foi acionada.
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458170"
---
# <a name="isundecidedapprovalrequest"></a>IsUndecidedApprovalRequest

O elemento **IsUndecidedApprovalRequest** especifica se uma mensagem de solicitação de aprovação foi acionada. 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **IsUndecidedApprovalRequest** será **true** se uma mensagem de solicitação de aprovação não tiver sido acionada. Um valor **false** indica que a solicitação de aprovação foi decidida. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[ApprovalRequestData](approvalrequestdata.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

