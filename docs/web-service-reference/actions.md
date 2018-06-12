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
description: O elemento de ações representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751040"
---
# <a name="actions"></a>Ações

O elemento de **ações** representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |Representa as categorias que estão marcadas em mensagens de email.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifica a ID da pasta que serão copiados para itens de email.  <br/> |
|[Delete](delete.md) <br/> |Indica se as mensagens devem ser movidos para a pasta Itens excluídos.  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Indica os endereços de email ao qual as mensagens devem ser encaminhadas como anexos.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Indica os endereços de email ao qual as mensagens devem ser encaminhadas.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Especifica a importância que deve ser marcada em mensagens.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Indica se as mensagens devem ser marcados como lidos.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifica a ID da pasta que serão movidos para itens de email.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Indica se as mensagens devem ser excluídos permanentemente e não são salvas na pasta Itens excluídos.  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Indica os endereços de email para os quais as mensagens devem ser redirecionados.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Indica os números de telefone celular para o qual um alerta do serviço SMS (Short Message) será enviado.  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Indica. a ID da mensagem modelo que deve ser enviado como uma resposta às mensagens de entrada.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Indica se as regras subsequentes devem ser avaliadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma única regra na caixa de correio do usuário.  <br/> |
   
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

- [Condições](conditions.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

