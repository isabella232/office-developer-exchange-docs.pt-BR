---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: O elemento ReplyBody contém uma mensagem Out of Office (OOF) e o idioma usado para a mensagem.
ms.openlocfilehash: 75af64277467246c7edcc2a48708bbf3f3c95c48
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517949"
---
# <a name="replybody"></a>ReplyBody

O **elemento ReplyBody** contém uma mensagem Out of Office (OOF) e o idioma usado para a mensagem. 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 **ReplyBody**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|xml:lang  <br/> |Especifica o idioma usado no conteúdo **ReplyBody.** Esse atributo é opcional. Os valores possíveis desse atributo são definidos pelo IETF RFC 3066.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Message (Availability)](message-availability.md) <br/> |Contém a resposta OOF (fora do escritório).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OutOfOffice](outofoffice.md) <br/> |Define a mensagem de resposta OOF e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento é obrigatório.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

