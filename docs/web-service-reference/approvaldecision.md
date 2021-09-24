---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: O elemento ApprovalDecision especifica a decisão tomada em uma mensagem de solicitação de aprovação.
ms.openlocfilehash: 903b75f04255a19ebb7a9b4d0e47b685f22d4339
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517228"
---
# <a name="approvaldecision"></a>ApprovalDecision

O **elemento ApprovalDecision** especifica a decisão tomada em uma mensagem de solicitação de aprovação. 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento ApprovalDecision** é 1 se aprovado e 2, se rejeitado. 
  
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

- [ApprovalRequestData](approvalrequestdata.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

