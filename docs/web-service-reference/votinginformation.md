---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: O elemento VotingInformation especifica as informações de votação em uma mensagem de votação e uma mensagem de solicitação de aprovação whereApproveandRejectare opções de votação.
ms.openlocfilehash: d946ba8c71d19c8cbb1befbe8c4e43e93590ccae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467743"
---
# <a name="votinginformation"></a>VotingInformation

O elemento **VotingInformation** especifica informações de votação em uma mensagem de votação e uma mensagem de solicitação de aprovação onde "aprovar" e "rejeitar" são as opções de votação. 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 **VotingInformationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[UserOptions](useroptions.md)  |  [VotingResponse](votingresponse.md)
  
### <a name="parent-elements"></a>Elementos pai

[Message](message-ex15websvcsotherref.md)
  
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
   
## <a name="see-also"></a>Também consulte



[Message](message-ex15websvcsotherref.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

