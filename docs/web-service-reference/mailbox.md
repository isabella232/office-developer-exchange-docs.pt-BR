---
title: Caixa de correio
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
description: O elemento Mailbox identifica um objeto do Active Directory habilitado para email.
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468198"
---
# <a name="mailbox"></a>Caixa de correio

O elemento **Mailbox** identifica um objeto do Active Directory habilitado para email. 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

**EmailAddresstype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddresstype)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Este elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio. Este elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento usado para a caixa de correio. O padrão é SMTP. Este elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Este elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Define uma solicitação para expandir uma lista de distribuição. <br/> <br/> A seguir está a expressão XPath para este elemento:` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Contém uma matriz de destinatários de um item.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Representa uma coleção de destinatários que receberão uma cópia da mensagem.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifica uma matriz de endereços de email aos quais as respostas devem ser enviadas.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
|[De](from.md) <br/> |Representa o destinatário de quem a mensagem foi enviada.  <br/> |
|[Organizador](organizer.md) <br/> |Representa o organizador de uma reunião.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Identifica as pastas padrão do Microsoft Exchange Server 2007.  <br/><br/>  A seguir estão as expressões XPath para este elemento: <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.  <br/> |
|[Participante](attendee.md) <br/> |Representa participantes e recursos de um item de calendário.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Define uma solicitação para adicionar pastas gerenciadas a uma caixa de correio.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes a uma caixa de correio.  <br/> |
|[Getdelegate](getdelegate.md) <br/> |Define uma solicitação para obter informações sobre representantes para uma caixa de correio.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Define uma solicitação para remover representantes de uma caixa de correio.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação para atualizar representantes em uma caixa de correio.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Descreve o representante em um cenário de acesso de representante.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Descreve o principal em um cenário de acesso de representante.  <br/> |
|[Membro](member-ex15websvcsotherref.md) <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Os elementos [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) e [ItemId](itemid.md) identificam uma caixa de correio ou lista de distribuição. 

O elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifica uma caixa de correio ou lista de distribuição por endereço SMTP. 

O elemento [ItemId](itemid.md) identifica uma caixa de correio por um identificador de item, que é associado a uma caixa de correio específica. 

O elemento [ItemId](itemid.md) não pode ser usado para enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta de contatos pública. Um erro será gerado se for usado em uma operação CreateItem, UpdateItem ou SendItem quando for feita uma tentativa de enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta pública de contatos. Use a operação ExpandDL para obter o endereço SMTP e, em seguida, enviar a mensagem usando o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) em vez do elemento [ItemId](itemid.md) . 
  
Outro elemento, [caixa de correio (disponibilidade)](mailbox-availability.md), fornece informações sobre operações de disponibilidade. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

