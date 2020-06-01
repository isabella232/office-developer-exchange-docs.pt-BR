---
title: Condições
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: O elemento Conditions identifica as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463199"
---
# <a name="conditions"></a>Condições

O elemento **Conditions** identifica as condições que, ao serem atendidas, acionarão as ações de regra para uma regra. 
  
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
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer nos cabeçalhos das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer nas propriedades **ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer na propriedade **from** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no corpo ou no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no assunto das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Especifica o sinalizador para o valor de ação que deve aparecer nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indica os endereços de email dos quais as mensagens de entrada devem ser enviadas para que a condição ou exceção seja aplicada.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Representa os nomes das contas de email a partir das quais as mensagens de entrada precisam ser agregadas para que a condição ou exceção seja aplicada.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indica se as mensagens de entrada precisam ter anexos para que a condição ou exceção seja aplicada.  <br/> |
|[Importance](importance.md) <br/> |Especifica a importância que é carimbada nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de aprovação para que a condição ou exceção seja aplicada.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indica se as mensagens de entrada devem ser encaminhamentos automáticos para que a condição ou exceção seja aplicada.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indica se as mensagens de entrada devem ser respostas automáticas para que a condição ou exceção seja aplicada.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indica se as mensagens de entrada devem ser criptografadas por S/MIME para que a condição ou exceção seja aplicada.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de reunião para que a condição ou exceção seja aplicada.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indica se as mensagens de entrada devem ser respostas de reunião para que a condição ou exceção seja aplicada.  <br/> |
|[IsNDR](isndr.md) <br/> |Indica se as mensagens de entrada devem ser notificações de falha na entrega (NDRs) para que a condição ou exceção seja aplicada.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indica se as mensagens de entrada devem ser controladas por permissões (protegidas por RMS) para que a condição ou exceção seja aplicada.  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indica se as mensagens de entrada devem ser recibos de leitura para que a condição ou exceção seja aplicada.  <br/> |
|[IsSigned](issigned.md) <br/> |Indica se as mensagens de entrada devem ser assinadas por S/MIME para que a condição ou exceção seja aplicada.  <br/> |
|[Iscaixa postal](isvoicemail.md) <br/> |Indica se as mensagens de entrada devem ser mensagens de caixa postal para que a condição ou exceção seja aplicada.  <br/> |
|[Doclasss](itemclasses.md) <br/> |Representa as classes de item que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Representa as classificações de mensagens que devem ser carimbadas nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indica se o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indica se o proprietário da caixa de correio deve estar na propriedade **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indica se o proprietário da caixa de correio deve ser a única na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indica os endereços de email para os quais as mensagens de entrada devem ter sido enviadas para que a condição ou exceção seja aplicada.  <br/> |
|[SentToMe](senttome.md) <br/> |Indica se o proprietário da caixa de correio deve estar na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indica se o proprietário da caixa de correio deve estar em uma propriedade **ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica a sensibilidade que deve ser carimbada nas mensagens de entrada para que a condição ou exceção seja aplicada.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Especifica o intervalo de datas no qual as mensagens de entrada precisam ser recebidas para que a condição ou exceção seja aplicada.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Especifica os tamanhos mínimo e máximo que as mensagens de entrada devem ter para que a condição ou exceção seja aplicada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regra (RuleType)](rule-ruletype.md) <br/> |Contém uma única regra e representa uma regra na caixa de correio de um usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Exceções](exceptions.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

