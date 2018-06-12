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
description: O elemento de UpdateInboxRules define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837902"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

O elemento de **UpdateInboxRules** define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor. 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **UpdateInboxRulesRequestType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Representa o endereço SMTP do usuário cujas regras de caixa de entrada devem ser criados, modificados ou excluídos.  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Indica se deseja remover o blob de regra do Microsoft Outlook.  <br/> |
|[Operations](operations.md) <br/> |Contém uma matriz das operações de regra que podem ser executadas em uma caixa de entrada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação UpdateInboxRules](updateinboxrules-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

