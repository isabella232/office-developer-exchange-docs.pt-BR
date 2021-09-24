---
title: Mailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: O elemento Mailbox identifica um objeto Active Directory habilitado para email.
ms.openlocfilehash: 8065c0472c3b847d538422aa77cd93f75d919a9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535000"
---
# <a name="mailbox"></a>Mailbox

O **elemento Mailbox** identifica um objeto Active Directory habilitado para email. 
  
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

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item de um contato ou lista de distribuição privada para destinatários da pasta de contatos de um usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExpandDL](expanddl.md) <br/> |Define uma solicitação para expandir uma lista de distribuição. <br/> <br/> Veja a seguir a expressão XPath para este elemento: ` /ExpandDL ` <br/> |
|[ToRecipients](torecipients.md) <br/> |Contém uma matriz de destinatários de um item.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Representa uma coleção de destinatários que receberão uma cópia da mensagem.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Representa uma coleção de destinatários para receber uma cópia de carbono cego (Cc) de um email.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifica uma matriz de endereços de email para os quais as respostas devem ser enviadas.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
|[De](from.md) <br/> |Representa o destinatário de quem a mensagem foi enviada.  <br/> |
|[Organizador](organizer.md) <br/> |Representa o organizador de uma reunião.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> | Identifica as pastas Microsoft Exchange Server 2007 padrão.  <br/><br/>  Veja a seguir as expressões XPath para este elemento: <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |Contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.  <br/> |
|[Attendee](attendee.md) <br/> |Representa participantes e recursos para um item de calendário.  <br/> |
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Define uma solicitação para adicionar pastas gerenciadas a uma caixa de correio.  <br/> |
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes a uma caixa de correio.  <br/> |
|[GetDelegate](getdelegate.md) <br/> |Define uma solicitação para obter informações sobre representantes para uma caixa de correio.  <br/> |
|[RemoveDelegate](removedelegate.md) <br/> |Define uma solicitação para remover representantes de uma caixa de correio.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação para atualizar representantes em uma caixa de correio.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Descreve o representante em um cenário de acesso de representante.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Descreve a entidade principal em um cenário de acesso de representante.  <br/> |
|[Membro](member-ex15websvcsotherref.md) <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Os [elementos EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) e [ItemId](itemid.md) identificam uma caixa de correio ou uma lista de distribuição. 

O [elemento EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) identifica uma caixa de correio ou uma lista de distribuição por endereço SMTP. 

O [elemento ItemId](itemid.md) identifica uma caixa de correio por um identificador de item, que é associado a uma caixa de correio específica. 

O [elemento ItemId](itemid.md) não pode ser usado para enviar uma mensagem para uma lista de distribuição ou um contato em uma pasta de contatos públicos. Um erro será lançado se for usado em uma operação CreateItem, UpdateItem ou SendItem quando for feita uma tentativa de enviar uma mensagem para uma lista de distribuição ou contato em uma pasta pública de contatos. Use a operação ExpandDL para obter o endereço SMTP e, em seguida, enviar a mensagem usando o [elemento EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) em vez do [elemento ItemId.](itemid.md) 
  
Outro elemento, [Mailbox (Availability),](mailbox-availability.md)fornece informações para operações de disponibilidade. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

