---
title: Ações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: O elemento Actions representa o conjunto de ações que estão disponíveis para serem tomadas em uma mensagem quando as condições são atendidas.
ms.openlocfilehash: 7f6608af5b8a9eb2772228a638fc42b9558f1e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546858"
---
# <a name="actions"></a>Ações

O **elemento Actions** representa o conjunto de ações que estão disponíveis para serem tomadas em uma mensagem quando as condições são atendidas. 
  
[Rule (RuleType)](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |Representa as categorias que são carimbadas em mensagens de email.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifica a ID da pasta para a onde os itens de email serão copiados.  <br/> |
|[Delete](delete.md) <br/> |Indica se as mensagens devem ser movidas para a pasta Itens Excluídos.  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser encaminhadas como anexos.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser encaminhadas.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Especifica a importância que deve ser carimbada nas mensagens.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Indica se as mensagens devem ser marcadas como leitura.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifica a ID da pasta para a onde os itens de email serão movidos.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Indica se as mensagens devem ser excluídas permanentemente e não salvas na pasta Itens Excluídos.  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser redirecionadas.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Indica os números de telefone celular para os quais um alerta sms deve ser enviado.  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Indica. a ID da mensagem de modelo que deve ser enviada como uma resposta às mensagens de entrada.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Indica se as regras subsequentes devem ser avaliadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule (RuleType)](rule-ruletype.md) <br/> |Representa uma única regra na caixa de correio de um usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [Condições](conditions.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

