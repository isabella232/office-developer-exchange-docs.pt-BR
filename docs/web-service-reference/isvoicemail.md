---
title: IsVoicemail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: O elemento IsVoicemail indica se as mensagens de entrada devem ser mensagens de caixa postal na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 513498301aa65eaf0cac5769c940eeedf5c9e629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824136"
---
# <a name="isvoicemail"></a>IsVoicemail

O elemento **IsVoicemail** indica se as mensagens de entrada devem ser mensagens de caixa postal na ordem para a condição ou uma exceção a ser aplicado. 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** indica que a mensagem deve ser uma mensagem de voz na ordem para a condição ou uma exceção a ser aplicado. Um valor **false** indica que a mensagem não deve ser uma mensagem de voz na ordem para a condição ou uma exceção a ser aplicado. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

