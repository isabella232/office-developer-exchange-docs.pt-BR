---
title: FieldUri (regra)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: O elemento FieldURI Especifica o URI para o campo de regra que causou o erro de validação.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752237"
---
# <a name="fielduri-rule"></a>FieldUri (regra)

O elemento **FieldURI** Especifica o URI para o campo de regra que causou o erro de validação. 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Erro](error.md) <br/> |Representa um erro de validação exclusivo em um valor da propriedade regra específica, o valor da propriedade predicado ou o valor da propriedade action.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto para esse elemento é restrito a uma das cadeias de caracteres seguintes:
  
- RuleId
    
- DisplayName
    
- Prioridade
    
- IsNotSupported
    
- Ações
    
- Condição: categorias
    
- Condição: ContainsBodyStrings
    
- Condição: ContainsHeaderStrings
    
- Condição: ContainsRecipientStrings
    
- Condição: ContainsSenderStrings
    
- Condição: ContainsSubjectOrBodyStrings
    
- Condição: ContainsSubjectStrings
    
- Condição: FlaggedForAction
    
- Condição: FromAddresses
    
- Condição: FromConnectedAccounts
    
- Condição: HasAttachments
    
- Condição: importância
    
- Condição: IsApprovalRequest
    
- Condição: IsAutomaticForward
    
- Condição: IsAutomaticReply
    
- Condição: IsEncrypted
    
- Condição: IsMeetingRequest
    
- Condição: IsMeetingResponse
    
- Condição: IsNDR
    
- Condição: IsPermissionControlled
    
- Condição: IsReadReceipt
    
- Condição: IsSigned
    
- Condição: IsVoicemail
    
- Condição: ItemClasses
    
- Condição: MessageClassifications
    
- Condição: NotSentToMe
    
- Condição: SentCcMe
    
- Condição: SentOnlyToMe
    
- Condição: SentToAddresses
    
- Condição: SentToMe
    
- Condição: SentToOrCcMe
    
- Condição: sensibilidade
    
- Condição: WithinDateRange
    
- Condição: WithinSizeRange
    
- Exceção: categorias
    
- Exceção: ContainsBodyStrings
    
- Exceção: ContainsHeaderStrings
    
- Exceção: ContainsRecipientStrings
    
- Exceção: ContainsSenderStrings
    
- Exceção: ContainsSubjectOrBodyStrings
    
- Exceção: ContainsSubjectStrings
    
- Exceção: FlaggedForAction
    
- Exceção: FromAddresses
    
- Exceção: FromConnectedAccounts
    
- Exceção: HasAttachments
    
- Exceção: importância
    
- Exceção: IsApprovalRequest
    
- Exceção: IsAutomaticForward
    
- Exceção: IsAutomaticReply
    
- Exceção: IsEncrypted
    
- Exceção: IsMeetingRequest
    
- Exceção: IsMeetingResponse
    
- Exceção: IsNDR
    
- Exceção: IsPermissionControlled
    
- Exceção: IsReadReceipt
    
- Exceção: IsSigned
    
- Exceção: IsVoicemail
    
- Exceção: ItemClasses
    
- Exceção: MessageClassifications
    
- Exceção: NotSentToMe
    
- Exceção: SentCcMe
    
- Exceção: SentOnlyToMe
    
- Exceção: SentToAddresses
    
- Exceção: SentToMe
    
- Exceção: SentToOrCcMe
    
- Exceção: sensibilidade
    
- Exceção: WithinDateRange
    
- Exceção: WithinSizeRange
    
- Ação: AssignCategories
    
- Ação: CopyToFolder
    
- Ação: excluir
    
- Ação: ForwardAsAttachmentToRecipients
    
- Ação: ForwardToRecipients
    
- Ação: MarkImportance
    
- Ação: MarkAsRead
    
- Ação: MoveToFolder
    
- Ação: PermanentDelete
    
- Ação: RedirectToRecipients
    
- Ação: SendSMSAlertToRecipients
    
- Ação: ServerReplyWithMessage
    
- Ação: StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- Condições
    
- Exceções
    
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

