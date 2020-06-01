---
title: Entrada (PhysicalAddress)
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
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: O elemento ENTRY descreve um único endereço físico para um item de contato.
ms.openlocfilehash: 5e8343e9abebeeff8c2b81327b2e0f4ddcf45364
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459627"
---
# <a name="entry-physicaladdress"></a>Entrada (PhysicalAddress)

O elemento **entry** descreve um único endereço físico para um item de contato. 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 **PhysicalAddressDictionaryEntryType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Key** <br/> | Identifica um endereço físico.<br/><br/> Estes são os valores possíveis para este atributo:<br/>  <br/>-Business  <br/>-Home  <br/>-Outros  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[123](street.md) <br/> |Representa um endereço de um item de contato.  <br/> |
|[Cidade](city.md) <br/> |Representa o nome da cidade que está associado a um contato.  <br/> |
|[State](state-ex15websvcsotherref.md) <br/> |Representa o estado de residência de um item de contato.  <br/> |
|[CountryOrRegion](countryorregion.md) <br/> |Representa o país ou a região de um determinado endereço físico.  <br/> |
|[PostalCode](postalcode.md) <br/> |Representa o código postal de um item de contato.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contém uma coleção de endereços físicos associados a um contato.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando contatos (serviços Web do Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Atualizando contatos](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Excluindo contatos](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

