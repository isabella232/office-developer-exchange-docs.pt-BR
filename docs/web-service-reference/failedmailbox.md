---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: O elemento FailedMailbox especifica a mensagem de erro de uma caixa de correio que falhou na pesquisa.
ms.openlocfilehash: 5e2bfbce5da35ecacd1757a9c612ed226af963ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535255"
---
# <a name="failedmailbox"></a>FailedMailbox

O **elemento FailedMailbox** especifica a mensagem de erro de uma caixa de correio que falhou na pesquisa. 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 **FailedSearchMailboxType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Mailbox (string)](mailbox-string.md) <br/> |Contém um identificador para a caixa de correio.  <br/> |
|[ErrorCode (int)](errorcode-int.md) <br/> |Especifica o código de erro da caixa de correio que falhou na pesquisa.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Representa o motivo do erro de validação.  <br/> |
|[IsArchive](isarchive.md) <br/> |Especifica um valor Boolean que indica se a caixa de correio é um arquivo morto.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FailedMailboxes](failedmailboxes.md) <br/> |Especifica uma matriz de caixas de correio com falha.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

