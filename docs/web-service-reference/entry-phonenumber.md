---
title: Entrada (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: O elemento de entrada representa um número de telefone de um contato.
ms.openlocfilehash: 3953488fb0b57fcf01c2fb99039478bbe03c7f5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752085"
---
# <a name="entry-phonenumber"></a>Entrada (PhoneNumber)

O elemento de **entrada** representa um número de telefone de um contato. 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Key** <br/> | Identifica o número de telefone. O atributo de chave é do tipo **PhoneNumberKeyType**.<br/><br/> Estes são os valores possíveis para este atributo:<br/><br/>-AssistantPhone  <br/>-BusinessFax  <br/>-Telefone comercial  <br/>-BusinessPhone2  <br/>-O retorno de chamada  <br/>-Telefone do carro  <br/>-CompanyMainPhone  <br/>-HomeFax  <br/>-HomePhone  <br/>-HomePhone2  <br/>-Isdn  <br/>-MobilePhone  <br/>-OtherFax  <br/>-OtherTelephone  <br/>-Pager  <br/>-PrimaryPhone  <br/>-RadioPhone  <br/>-Telex  <br/>-TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Representa uma coleção de números de telefone de um contato.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa um número de telefone.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criação de contatos (serviços Web do Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Atualizar contatos](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Excluindo contatos](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

