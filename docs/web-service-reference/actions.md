---
title: Ações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: O elemento Actions representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465062"
---
# <a name="actions"></a>Ações

O elemento **Actions** representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas. 
  
[Regra (RuleType)](rule-ruletype.md)
  
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
|[AssignCategories](assigncategories.md) <br/> |Representa as categorias carimbadas nas mensagens de email.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifica a ID da pasta para a qual os itens de email serão copiados.  <br/> |
|[Delete](delete.md) <br/> |Indica se as mensagens devem ser movidas para a pasta itens excluídos.  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser encaminhadas como anexos.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser encaminhadas.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Especifica a importância a ser carimbada nas mensagens.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Indica se as mensagens devem ser marcadas como lidas.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifica a ID da pasta para a qual os itens de email serão movidos.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Indica se as mensagens devem ser excluídas permanentemente e não são salvas na pasta itens excluídos.  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Indica os endereços de email aos quais as mensagens devem ser redirecionadas.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Indica os números de telefone celular para os quais um alerta de serviço de mensagem curta (SMS) deve ser enviado.  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Informa. a ID da mensagem de modelo a ser enviada como uma resposta a mensagens de entrada.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Indica se as regras subsequentes serão avaliadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma única regra na caixa de correio de um usuário.  <br/> |
   
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
   
## <a name="see-also"></a>Confira também

- [Condições](conditions.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

