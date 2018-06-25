---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: O elemento SendPrompt Especifica o tipo de ação permitida para uma opção de votação.
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825346"
---
# <a name="sendprompt"></a>SendPrompt

O elemento **SendPrompt** Especifica o tipo de ação permitida para uma opção de votação. 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **SendPrompt** é uma ação de opção de votação. A tabela a seguir lista os valores possíveis para esse elemento. 
  
****

|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Nenhuma ação.  <br/> |
|Enviar  <br/> |A resposta é enviada imediatamente.  <br/> |
|VotingOption  <br/> |O aprovador pode inserir comentários ao aprovar ou rejeitar.  <br/> |
   
## <a name="remarks"></a>Comentários

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



[VotingOptionData](votingoptiondata.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

