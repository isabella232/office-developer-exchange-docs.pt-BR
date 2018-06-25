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
description: O elemento de condições identifica as condições que, quando atendida, irá disparar as ações de regra para uma regra.
ms.openlocfilehash: f66777e82892122c4c7dac45bdef3c42f5c4a577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751418"
---
# <a name="conditions"></a>Condições

O elemento de **condições** identifica as condições que, quando atendida, irá disparar as ações de regra para uma regra. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contém as categorias que devem ser aplicadas a uma mensagem de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no corpo de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer nos cabeçalhos de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer em Propriedades no **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer na propriedade **** das mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no corpo ou o assunto de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indica as cadeias de caracteres que devem aparecer no assunto do mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Especifica o sinalizador para o valor de ação que deverá aparecer nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indica os endereços de email do qual as mensagens de entrada devem ser enviadas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Representa os nomes de conta de email do qual mensagens recebidas precisam ter foram agregados na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indica se as mensagens recebidas precisam ter anexos em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[Importância](importance.md) <br/> |Especifica a importância que é marcada nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de aprovação em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indica se as mensagens de entrada devem ser encaminhamentos automáticos na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indica se as mensagens recebidas devem ser as respostas automáticas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indica se as mensagens de entrada devem ser S/MIME criptografada em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indica se as mensagens de entrada devem ser solicitações de reunião na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indica se as mensagens de entrada devem ser respostas de reunião na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsNDR](isndr.md) <br/> |Indica se as mensagens recebidas devem ser relatórios de falha na entrega (NDRs) em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indica se as mensagens de entrada devem ser controlado de permissão (protegida por RMS) na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indica se as mensagens de entrada devem ser confirmações de leitura na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsSigned](issigned.md) <br/> |Indica se as mensagens de entrada devem ser QUE S/MIME assinadas em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Indica se as mensagens de entrada devem ser mensagens de caixa postal na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Representa as classes de item que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Representa as classificações de mensagem que devem ser marcadas em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indica se o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indica se o proprietário da caixa de correio deve ser na propriedade **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indica se o proprietário da caixa de correio deve ser a única pessoa na propriedade **ToRecipients** de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indica os endereços de email que precisam foram enviadas em ordem para a condição ou exceção para aplicar a mensagens de entrada.  <br/> |
|[SentToMe](senttome.md) <br/> |Indica se o proprietário da caixa de correio deve ser na propriedade **ToRecipients** de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indica se o proprietário da caixa de correio deve ser na propriedade um **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica a sensibilidade que deve ser marcada em mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Especifica o intervalo de datas dentro do qual as mensagens recebidas precisará foram recebidos em ordem para a condição ou uma exceção a ser aplicado.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regra (RuleType)](rule-ruletype.md) <br/> |Contém uma única regra e representa uma regra de caixa de correio do usuário.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Exceções](exceptions.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

