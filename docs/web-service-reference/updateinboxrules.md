---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: O elemento UpdateInboxRules define uma solicitação para atualizar as regras de Caixa de Entrada em uma caixa de correio no armazenamento do servidor.
ms.openlocfilehash: 823763efc9f9dfe621ccf05356f7e0f3c7bace14
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541704"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

O **elemento UpdateInboxRules** define uma solicitação para atualizar as regras de Caixa de Entrada em uma caixa de correio no armazenamento do servidor. 
  
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
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Representa o endereço SMTP do usuário cujas regras de Caixa de Entrada devem ser criadas, modificadas ou excluídas.  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Indica se é preciso remover o blob Outlook regra da Microsoft.  <br/> |
|[Operations](operations.md) <br/> |Contém uma matriz de operações de regra que podem ser executadas em uma Caixa de Entrada.  <br/> |
   
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
   
## <a name="see-also"></a>Confira também



[Operação UpdateInboxRules](updateinboxrules-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

