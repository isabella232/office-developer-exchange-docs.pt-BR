---
title: IsArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b89d8a78-5c18-4547-aaf4-4b16a93190a7
description: O elemento IsArchive especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto.
ms.openlocfilehash: 269cb614ad9402a266b2ed521c4f485b3f43b1fb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514561"
---
# <a name="isarchive"></a>IsArchive

O **elemento IsArchive** especifica um valor Boolean que indica se a caixa de correio é uma caixa de correio de arquivo morto. 
  
```XML
<IsArchive>true | false</IsArchive>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[FailedMailbox](failedmailbox.md)  |  [RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento IsArchive** indica que a caixa de correio de destino é uma caixa de correio de arquivo morto. Um valor false indica **que** a caixa de correio de destino não é uma caixa de correio de arquivo morto. 
  
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

