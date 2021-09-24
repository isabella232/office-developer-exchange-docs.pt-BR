---
title: FieldUri (Rule)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: O elemento FieldURI especifica o URI para o campo de regra que causou o erro de validação.
ms.openlocfilehash: c1390f6643614216fa86053368ba012cd0883ff7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513728"
---
# <a name="fielduri-rule"></a>FieldUri (Rule)

O **elemento FieldURI** especifica o URI para o campo de regra que causou o erro de validação. 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Erro](error.md) <br/> |Representa um único erro de validação em um determinado valor de propriedade de regra, valor da propriedade predicado ou valor da propriedade action.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para esse elemento é restrito a uma das seguintes cadeias de caracteres:
  
- RuleId
    
- DisplayName
    
- Prioridade
    
- IsNotSupported
    
- Ações
    
- Condição:Categorias
    
- Condition:ContainsBodyStrings
    
- Condition:ContainsHeaderStrings
    
- Condition:ContainsRecipientStrings
    
- Condition:ContainsSenderStrings
    
- Condition:ContainsSubjectOrBodyStrings
    
- Condition:ContainsSubjectStrings
    
- Condition:FlaggedForAction
    
- Condition:FromAddresses
    
- Condition:FromConnectedAccounts
    
- Condition:HasAttachments
    
- Condição:Importância
    
- Condition:IsApprovalRequest
    
- Condition:IsAutomaticForward
    
- Condition:IsAutomaticReply
    
- Condition:IsEncrypted
    
- Condition:IsMeetingRequest
    
- Condition:IsMeetingResponse
    
- Condition:IsNDR
    
- Condition:IsPermissionControlled
    
- Condition:IsReadReceipt
    
- Condition:IsSigned
    
- Condition:IsVoicemail
    
- Condition:ItemClasses
    
- Condition:MessageClassifications
    
- Condition:NotSentToMe
    
- Condition:SentCcMe
    
- Condition:SentOnlyToMe
    
- Condition:SentToAddresses
    
- Condition:SentToMe
    
- Condition:SentToOrCcMe
    
- Condição:Sensibilidade
    
- Condition:WithinDateRange
    
- Condição:WithinSizeRange
    
- Exception:Categories
    
- Exception:ContainsBodyStrings
    
- Exception:ContainsHeaderStrings
    
- Exception:ContainsRecipientStrings
    
- Exception:ContainsSenderStrings
    
- Exception:ContainsSubjectOrBodyStrings
    
- Exception:ContainsSubjectStrings
    
- Exception:FlaggedForAction
    
- Exception:FromAddresses
    
- Exception:FromConnectedAccounts
    
- Exception:HasAttachments
    
- Exception:Importance
    
- Exception:IsApprovalRequest
    
- Exception:IsAutomaticForward
    
- Exception:IsAutomaticReply
    
- Exception:IsEncrypted
    
- Exception:IsMeetingRequest
    
- Exception:IsMeetingResponse
    
- Exception:IsNDR
    
- Exception:IsPermissionControlled
    
- Exception:IsReadReceipt
    
- Exception:IsSigned
    
- Exception:IsVoicemail
    
- Exception:ItemClasses
    
- Exception:MessageClassifications
    
- Exception:NotSentToMe
    
- Exception:SentCcMe
    
- Exception:SentOnlyToMe
    
- Exception:SentToAddresses
    
- Exception:SentToMe
    
- Exception:SentToOrCcMe
    
- Exception:Sensitivity
    
- Exception:WithinDateRange
    
- Exception:WithinSizeRange
    
- Action:AssignCategories
    
- Action:CopyToFolder
    
- Action:Delete
    
- Action:ForwardAsAttachmentToRecipients
    
- Action:ForwardToRecipients
    
- Action:MarkImportance
    
- Action:MarkAsRead
    
- Action:MoveToFolder
    
- Action:PermanentDelete
    
- Action:RedirectToRecipients
    
- Action:SendSMSAlertToRecipients
    
- Action:ServerReplyWithMessage
    
- Action:StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- Condições
    
- Exceções
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

