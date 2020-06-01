---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: O elemento UpdateInboxRules define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456357"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

O elemento **UpdateInboxRules** define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor. 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **UpdateInboxRulesRequestType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser criadas, modificadas ou excluídas.  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Indica se o blob de regra do Microsoft Outlook deve ser removido.  <br/> |
|[Operations](operations.md) <br/> |Contém uma matriz de operações de regra que podem ser executadas em uma caixa de entrada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Operação UpdateInboxRules](updateinboxrules-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

