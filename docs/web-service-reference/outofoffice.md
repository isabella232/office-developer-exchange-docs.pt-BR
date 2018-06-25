---
title: Fora do escritório
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: O elemento de fora do escritório representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.
ms.openlocfilehash: 4e1e06ee332c44aeba03e1343c8c3258a2c9631e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824675"
---
# <a name="outofoffice"></a>Fora do escritório

O elemento de **fora do escritório** representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta. 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

 **OutOfOfficeMailTip**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReplyBody](replybody.md) <br/> |Contém uma mensagem de fora do escritório (OOF) e o idioma usado para a mensagem.  <br/> |
|[Duração (UserOofSettings)](duration-useroofsettings.md) <br/> |Contém a duração em que o status de ausência temporária será habilitado se o elemento [OofState](oofstate.md) for definido como agendado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Dicas de email](mailtips.md) <br/> |Representa os valores para os vários tipos de dicas de email.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

