---
title: BusinessPhoneNumbers2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f335ea74-9b5b-4224-9475-40ef33fe76bd
description: O elemento BusinessPhoneNumbers2 especifica uma matriz de elementos BusinessPhoneNumber2 e os identificadores de suas atribuições de origem para a persona associada.
ms.openlocfilehash: be4f2d80846f026b5f19eab1ae23fc4ad42fddc8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545598"
---
# <a name="businessphonenumbers2"></a>BusinessPhoneNumbers2

O **elemento BusinessPhoneNumbers2** especifica uma matriz de elementos **BusinessPhoneNumber2** e os identificadores de suas atribuições de origem para a persona associada. 
  
```XML
<BusinessPhoneNumbers2>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers2>
```

 **ArrayOfPhoneNumberAttributedValuesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md) <br/> |Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Especifica uma matriz de atribuições para seu elemento **Value** associado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pessoal](persona.md) <br/> |Especifica um conjunto de dados de persona retornados por uma **solicitação GetPersona.**  <br/> |
   
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

