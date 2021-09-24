---
title: CallbackPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: O elemento CallbackPhones especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para a persona associada.
ms.openlocfilehash: 99a3cec041886a40d4f25fc1c0d272111aae7331
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514750"
---
# <a name="callbackphones"></a>CallbackPhones

O **elemento CallbackPhones** especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para a persona associada. 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
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

