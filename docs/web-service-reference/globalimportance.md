---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: O elemento GlobalImportance contém a importância agregada para todos os itens de conversa em uma caixa de correio.
ms.openlocfilehash: c760168afa3edac20ca0ae7bc677610d8456d178
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459444"
---
# <a name="globalimportance"></a>GlobalImportance

O elemento **GlobalImportance** contém a importância agregada para todos os itens de conversa em uma caixa de correio. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversas](conversations-ex15websvcsotherref.md)
  
[Conversa (Conversatype)](conversation-conversationtype.md)
  
[GlobalImportance](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 **ImportanceChoicesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversa (Conversatype)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Estes são os valores possíveis para este elemento:
  
- Baixo
    
- Normal
    
- Alta
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)
  
[Operação ApplyConversationAction](applyconversationaction-operation.md)


[Conversas no EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

