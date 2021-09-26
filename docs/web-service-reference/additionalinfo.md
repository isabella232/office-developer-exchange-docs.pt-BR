---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: O elemento AdditionalInfo especifica informações adicionais sobre o status de espera de uma caixa de correio.
ms.openlocfilehash: d8b707fb04ffe91d5c7aa793c6b56c8bb048f160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544315"
---
# <a name="additionalinfo"></a>AdditionalInfo

O **elemento AdditionalInfo** especifica informações adicionais sobre o status de espera de uma caixa de correio. 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs:string**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |Especifica o status de espera da caixa de correio.  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |Especifica detalhes de um item que não pode ser indexado.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento AdditionalInfo é informações adicionais sobre o status de espera de uma caixa de correio.
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional.
  
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

