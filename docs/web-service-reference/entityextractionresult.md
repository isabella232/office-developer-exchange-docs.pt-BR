---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: O elemento EntityExtractionResult especifica a propriedade EntityExtractionResult de um item.
ms.openlocfilehash: f2f069717a5862adff3349090c35f95499d135f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456952"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

O elemento **EntityExtractionResult** especifica a propriedade **EntityExtractionResult** de um item. 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 **EntityExtractionResultType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Endereços (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |Especifica uma matriz de elementos **AddressEntity** .  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |Especifica uma matriz de elementos **MeetingSuggestion** .  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |Especifica uma matriz de elementos **TaskSuggestion** .  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |Especifica uma matriz de entidades de endereço de email.  <br/> |
|[Contatos (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Especifica uma matriz de contatos.  <br/> |
|[URLs (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Especifica uma matriz de URLs.  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |Especifica uma matriz de números de telefone.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Item](item.md) <br/> |Representa um item genérico no repositório do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Também consulte



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

