---
title: Mailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: O elemento de caixa de correio identifica um objeto do Active Directory habilitado para email.
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824258"
---
# <a name="mailbox"></a>Mailbox

O elemento de **caixa de correio** identifica um objeto do Active Directory habilitado para email. 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddressType)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento que é usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Define uma solicitação para expandir uma lista de distribuição. <br/> <br/> Este é a expressão XPath para esse elemento:` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Contém uma matriz de destinatários de um item.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Representa uma coleção dos destinatários que receberão uma cópia da mensagem.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifica uma matriz de endereços de email para o qual as respostas devem ser enviadas.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
|[From](from.md) <br/> |Representa o destinatário de quem a mensagem foi enviada.  <br/> |
|[Organizer](organizer.md) <br/> |Representa o organizador de uma reunião.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Identifica as pastas padrão do Microsoft Exchange Server 2007.  <br/><br/>  A seguir estão as expressões XPath para esse elemento: <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.  <br/> |
|[Attendee](attendee.md) <br/> |Representa os participantes e recursos para um item de calendário.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Define uma solicitação para adicionar pastas gerenciadas para uma caixa de correio.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes para uma caixa de correio.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Define uma solicitação para remover representantes de uma caixa de correio.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação de atualização de representantes em uma caixa de correio.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Descreve o delegado em um cenário de acesso de representante.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Descreve a entidade em um cenário de acesso de representante.  <br/> |
|[Membro](member-ex15websvcsotherref.md) <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

Os elementos [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) e [ItemId](itemid.md) identificam uma lista de distribuição ou de caixa de correio. 

O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifica uma lista de distribuição ou de caixa de correio pelo endereço SMTP. 

O elemento [ItemId](itemid.md) identifica uma caixa de correio por um identificador de item, que é associado a uma caixa de correio específica. 

O elemento [ItemId](itemid.md) não pode ser usado para enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta pública de contatos. Um erro será lançado se isso for usado em uma operação de CreateItem, UpdateItem ou SendItem quando é feita uma tentativa para enviar uma mensagem a uma lista de distribuição ou um contato em uma pasta pública de contatos. Use a operação ExpandDL para obter o endereço SMTP e, em seguida, envie a mensagem usando o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) em vez do elemento [ItemId](itemid.md) . 
  
Outro elemento, [a caixa de correio (disponibilidade)](mailbox-availability.md), fornece informações para operações de disponibilidade. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

