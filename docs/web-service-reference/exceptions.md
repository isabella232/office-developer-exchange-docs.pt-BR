---
title: Exceções
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: O elemento Exceptions identifica as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada.
ms.openlocfilehash: 5c92613aa871a200cf790e0709ba71280b226807
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524263"
---
# <a name="exceptions"></a>Exceções

O **elemento Exceptions** identifica as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de Caixa de Entrada. 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 **RulePredicatesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contém as categorias que devem ser aplicadas a uma mensagem de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no corpo das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer nos headers de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer nas propriedades **ToRecipients** ou **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer na **propriedade From** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no corpo ou no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Especifica o sinalizador do valor de ação que deve aparecer nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indica os endereços de email dos quais as mensagens de entrada devem ser enviadas para que a condição ou exceção seja aplicada.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Representa os nomes de conta de email dos quais as mensagens de entrada têm que ser agregadas para que a condição ou exceção seja aplicada.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indica se as mensagens de entrada têm que ter anexos para que a condição ou exceção seja aplicada.  <br/> |
|[Importance](importance.md) <br/> |Especifica a importância que é carimbada em mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de aprovação para que a condição ou exceção seja aplicada.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indica se as mensagens de entrada devem ser encaminhadas automáticas para que a condição ou exceção seja aplicada.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indica se as mensagens de entrada devem ser respostas automáticas para que a condição ou exceção seja aplicada.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indica se as mensagens de entrada devem ser criptografadas S/MIME para que a condição ou exceção seja aplicada.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de reunião para que a condição ou exceção seja aplicada.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indica se as mensagens de entrada devem ser respostas de reunião para que a condição ou exceção seja aplicada.  <br/> |
|[IsNDR](isndr.md) <br/> |Indica se as mensagens de entrada devem ser NDRs (relatórios de não entrega) para que a condição ou exceção seja aplicada.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indica se as mensagens de entrada devem ser controladas por permissão (protegido por RMS) para que a condição ou exceção seja aplicada  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indica se as mensagens de entrada devem ser recibos de leitura para que a condição ou exceção seja aplicada.  <br/> |
|[IsSigned](issigned.md) <br/> |Indica se as mensagens de entrada devem ser assinadas por S/MIME para que a condição ou exceção seja aplicada.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Indica se as mensagens de entrada devem ser mensagens de caixa postal para que a condição ou exceção seja aplicada.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Representa as classes de item que devem ser carimbadas em mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Representa as classificações de mensagem que devem ser carimbadas em mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indica se o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indica se o proprietário da caixa de correio precisa estar na propriedade **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indica se o proprietário da caixa de correio deve ser o único na **propriedade ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indica os endereços de email para os que as mensagens de entrada têm que ter sido enviadas para que a condição ou exceção seja aplicada.  <br/> |
|[SentToMe](senttome.md) <br/> |Indica se o proprietário da caixa de correio precisa estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indica se o proprietário da caixa de correio precisa estar em uma **propriedade ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica a sensibilidade que deve ser carimbada em mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Especifica o intervalo de datas no qual as mensagens de entrada têm que ser recebidas para que a condição ou exceção seja aplicada.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Especifica os tamanhos mínimo e máximo que as mensagens de entrada devem estar para que a condição ou exceção seja aplicada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule (RuleType)](rule-ruletype.md) <br/> |Contém uma única regra e representa uma regra na caixa de correio de um usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Os predicados de regra são usados como condições de regra ou exceções.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Condições](conditions.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

