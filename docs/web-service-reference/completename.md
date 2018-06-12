---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: O elemento CompleteName representa o nome completo de um contato.
ms.openlocfilehash: 1f6c9ba68fe941f848d0e250a39aea6894fca61e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751406"
---
# <a name="completename"></a>CompleteName

O elemento **CompleteName** representa o nome completo de um contato. 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 **CompleteNameType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Title](title.md) <br/> |Representa o título de um contato.  <br/> |
|[FirstName](firstname.md) <br/> |Representa o nome do contato.  <br/> |
|[MiddleName](middlename.md) <br/> |Representa o nome do meio de um contato.  <br/> |
|[LastName](lastname.md) <br/> |Representa o último nome de um contato.  <br/> |
|[Suffix](suffix.md) <br/> |Representa um sufixo de nome de um contato.  <br/> |
|[Iniciais](initials.md) <br/> |Representa as iniciais de um contato.  <br/> |
|[FullName](fullname.md) <br/> |Representa o nome completo de um contato.  <br/> |
|[Apelido](nickname.md) <br/> |Representa o apelido de um contato.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Representa o nome usado no Japão para a ortografia pesquisável ou fonética de um nome japonês.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Representa o nome usado no Japão para a ortografia pesquisável ou fonética do japonês sobrenome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
   
## <a name="remarks"></a>Coment�rios

A propriedade [CompleteName](completename.md) é parte da forma [padrão](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx) . Na versão release inicial do Microsoft Exchange Server 2007, a propriedade [CompleteName](completename.md) é retornada pela [operação GetItem](getitem-operation.md), mas não a [operação FindItem](finditem-operation.md). Iniciando com o Exchange Server 2007 Service Pack 1 (SP1), a [operação FindItem](finditem-operation.md) também retorna a propriedade [CompleteName](completename.md) com a forma [padrão](https://msdn.microsoft.com/library/ExchangeWebServices.DefaultShapeNamesType.Default.aspx) . Essa alteração não afeta o esquema. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
  
[CompleteName](https://msdn.microsoft.com/library/ExchangeWebServices.ContactItemType.CompleteName.aspx)
  
[contactsCompleteName](https://msdn.microsoft.com/library/ExchangeWebServices.UnindexedFieldURIType.contactsCompleteName.aspx)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criação de contatos (serviços Web do Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

