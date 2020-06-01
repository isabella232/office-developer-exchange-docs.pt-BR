---
title: Contato (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: O elemento Contact especifica um contato no repositório unificado de contatos.
ms.openlocfilehash: e8ebc28456f8bfc26f5d790ac9ff278930041ea0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461517"
---
# <a name="contact-contacttype"></a>Contato (ContactType)

O elemento **Contact** especifica um contato no repositório unificado de contatos. 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 **ContactType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PersonName](personname.md) <br/> |Especifica o nome de um indivíduo.  <br/> |
|[BusinessName](businessname.md) <br/> |Especifica o nome de uma empresa.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Representa uma coleção de números de telefone de um contato.  <br/> |
|[URLs](urls.md) <br/> |Especifica uma matriz de URLs para uma pessoa.  <br/> |
|[EmailAddresses (ArrayOfExtractedEmailAddresses)](emailaddresses-arrayofextractedemailaddresses.md) <br/> |Especifica uma matriz de endereços de email extraídos.  <br/> |
|[Endereços (ArrayOfAddressesType)](addresses-arrayofaddressestype.md) <br/> |Especifica uma matriz de elementos de **endereço** .  <br/> |
|[Contactstring](contactstring.md) <br/> |Especifica o nome de exibição de um contato.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Contatos (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Especifica uma matriz de contatos.  <br/> |
   
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

