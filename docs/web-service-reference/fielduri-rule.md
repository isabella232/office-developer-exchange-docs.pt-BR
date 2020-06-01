---
title: FieldUri (regra)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: O elemento FieldURI especifica o URI para o campo de regra que causou o erro de validação.
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461244"
---
# <a name="fielduri-rule"></a>FieldUri (regra)

O elemento **FieldURI** especifica o URI para o campo de regra que causou o erro de validação. 
  
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
|[Erro](error.md) <br/> |Representa um único erro de validação em um valor de propriedade de regra específico, um valor da propriedade Predicate ou um valor da propriedade Action.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto para este elemento é restrito a uma das seguintes cadeias de caracteres:
  
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
    
- Condição: iscaixa postal
    
- Condição: doclasss
    
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
    
- Exceção: ispostal
    
- Exceção: doclasss
    
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
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

