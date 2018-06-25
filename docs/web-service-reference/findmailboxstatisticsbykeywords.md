---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: O elemento FindMailboxStatisticsByKeywords Especifica uma solicitação para pesquisar por palavra-chave estatísticas de caixa de correio.
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752285"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

O elemento **FindMailboxStatisticsByKeywords** Especifica uma solicitação para pesquisar por palavra-chave estatísticas de caixa de correio. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixas de correio (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |Contém uma matriz de caixas de correio afetadas pela retenção.  <br/> |
|[Palavras-chave](keywords-ex15websvcsotherref.md) <br/> |Especifica as palavras-chave para uma pesquisa.  <br/> |
|[Idioma](language.md) <br/> |Contém o idioma usado para a consulta de pesquisa.  <br/> |
|[Remetentes](senders.md) <br/> |Especifica uma matriz de endereços SMTP.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Especifica uma matriz de destinatários de uma mensagem.  <br/> |
|[FromDate](fromdate.md) <br/> |Especifica a data em que a mensagem foi enviada.  <br/> |
|[ToDate](todate.md) <br/> |Especifica a data em que a mensagem foi recebida.  <br/> |
|[MessageTypes](messagetypes.md) <br/> |Especifica uma matriz de mensagens a ser pesquisado.  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |Especifica se deve pesquisar em itens excluídos.  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |Especifica se é necessário incluir o arquivo pessoal na pesquisa.  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |Especifica se é necessário incluir os itens que não podem ser pesquisados.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

