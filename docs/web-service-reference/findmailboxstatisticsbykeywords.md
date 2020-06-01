---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: O elemento FindMailboxStatisticsByKeywords especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462525"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

O elemento **FindMailboxStatisticsByKeywords** especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave. 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 **FindMailboxStatisticsByKeywordsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixas de correio (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |Contém uma matriz de caixas de correio afetadas pela isenção.  <br/> |
|[Keywords](keywords-ex15websvcsotherref.md) <br/> |Especifica palavras-chave para uma pesquisa.  <br/> |
|[Language](language.md) <br/> |Contém o idioma usado para a consulta de pesquisa.  <br/> |
|[Remetentes](senders.md) <br/> |Especifica uma matriz de endereços SMTP.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Especifica uma matriz de destinatários de uma mensagem.  <br/> |
|[FromDate](fromdate.md) <br/> |Especifica a data em que a mensagem foi enviada.  <br/> |
|[ToDate](todate.md) <br/> |Especifica a data em que a mensagem foi recebida.  <br/> |
|[MessageType](messagetypes.md) <br/> |Especifica uma matriz de mensagens a serem pesquisadas.  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |Especifica se pesquisar em itens excluídos.  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |Especifica se é para incluir o arquivo morto pessoal na pesquisa.  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |Especifica se é para incluir itens que não podem ser pesquisados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

