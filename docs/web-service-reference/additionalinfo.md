---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: O elemento AdditionalInfo Especifica informações adicionais sobre o status de retenção de uma caixa de correio.
ms.openlocfilehash: 6fbe24d5d3e41f2ba9c81657b2c38240d10eefed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751057"
---
# <a name="additionalinfo"></a>AdditionalInfo

O elemento **AdditionalInfo** Especifica informações adicionais sobre o status de retenção de uma caixa de correio. 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs: String**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |Especifica o status de retenção da caixa de correio.  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |Especifica detalhes para um item que não pode ser indexado.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento AdditionalInfo é informações adicionais sobre o status de retenção de uma caixa de correio.
  
## <a name="remarks"></a>Coment�rios

Esse elemento é opcional.
  
Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

