---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: O elemento SendPrompt especifica o tipo de ação permitido para uma opção de votação.
ms.openlocfilehash: 32537210aadce91911d1fb5002fbafcaa70aa9ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532129"
---
# <a name="sendprompt"></a>SendPrompt

O **elemento SendPrompt** especifica o tipo de ação permitido para uma opção de votação. 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SendPrompt** é uma ação de opção de votação. A tabela a seguir lista os valores possíveis para esse elemento. 
  
****

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Nenhuma ação.  <br/> |
|Enviar  <br/> |A resposta é enviada imediatamente.  <br/> |
|VotingOption  <br/> |O aprovador pode inserir comentários durante a aprovação ou rejeição.  <br/> |
   
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



[VotingOptionData](votingoptiondata.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

