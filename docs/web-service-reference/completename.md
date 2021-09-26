---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: O elemento CompleteName representa o nome completo de um contato.
ms.openlocfilehash: 873d372657089d21e86025cdf7812659ac505491
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543552"
---
# <a name="completename"></a>CompleteName

O **elemento CompleteName** representa o nome completo de um contato. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Title](title.md) <br/> |Representa o título de um contato.  <br/> |
|[FirstName](firstname.md) <br/> |Representa o primeiro nome do contato.  <br/> |
|[MiddleName](middlename.md) <br/> |Representa o nome do meio de um contato.  <br/> |
|[LastName](lastname.md) <br/> |Representa o sobrenome de um contato.  <br/> |
|[Sufixo](suffix.md) <br/> |Representa um sufixo para o nome de um contato.  <br/> |
|[Iniciais](initials.md) <br/> |Representa as iniciais de um contato.  <br/> |
|[FullName](fullname.md) <br/> |Representa o nome completo de um contato.  <br/> |
|[Apelido](nickname.md) <br/> |Representa o apelido de um contato.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Representa o nome usado no Japão para a ortografia pesquisável ou phoneética de um nome japonês.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Representa o nome usado no Japão para a ortografia pesquisável ou phoneética de um sobrenome japonês.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
   
## <a name="remarks"></a>Comentários

A propriedade CompleteName faz parte da [forma](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) Padrão. Na versão inicial do Microsoft Exchange Server 2007, a propriedade CompleteName é retornada pela operação [GetItem](getitem-operation.md), mas não pela [operação FindItem](finditem-operation.md). A partir Exchange Server 2007 Service Pack 1 (SP1), a operação [FindItem](finditem-operation.md) também retorna a propriedade CompleteName com a [forma](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) Padrão. Essa alteração não afeta o esquema. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando contatos (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

