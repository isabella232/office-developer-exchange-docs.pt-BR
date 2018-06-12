---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: O elemento VotingInformation Especifica informações votação em uma mensagem de votação e whereApproveandRejectare de mensagem de solicitação de aprovação, as opções de votação.
ms.openlocfilehash: f11c25bb1f3a3c4781cfa6c51e11ff87af40c7f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838038"
---
# <a name="votinginformation"></a>VotingInformation

O elemento **VotingInformation** Especifica as informações de votação em uma mensagem de votação e a mensagem de solicitação de aprovação onde "Approve" e "Rejeitar" é as opções de votação. 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 **VotingInformationType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)
  
### <a name="parent-elements"></a>Elementos pai

[Mensagem](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Mensagem](message-ex15websvcsotherref.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

