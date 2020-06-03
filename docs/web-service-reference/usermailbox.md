---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: O elemento UserMailbox identifica uma caixa de correio de usuário.
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465314"
---
# <a name="usermailbox"></a>UserMailbox

O elemento **UserMailbox** identifica uma caixa de correio de usuário. 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **Usermailboxtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |O valor de texto do atributo **ID** é o identificador da caixa de correio.  <br/> |
|IsArchive  <br/> |O valor de texto do atributo **IsArchive** indica se a caixa de correio é uma caixa de correio de arquivo morto. Um valor de texto **true** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio de arquivo morto. Um valor **false** para o atributo **IsArchive** indica que a caixa de correio é uma caixa de correio principal.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Caixas de correio (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  |  [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |verdadeiro  <br/> |
   

