---
title: Scope (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: O elemento Scope especifica o escopo do relatório de controle de mensagens.
ms.openlocfilehash: 036ff1007c9e7ec9cc385f8df81c045b7b9335b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546123"
---
# <a name="scope-nonemptystringtype"></a>Scope (NonEmptyStringType)

O **elemento Scope** especifica o escopo do relatório de controle de mensagens. 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[FindMessageTrackingReport](findmessagetrackingreport.md)  |  [GetMessageTrackingReport](getmessagetrackingreport.md)
  
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento Scope.** 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Organização  <br/> |Os escopos de controle de mensagens abrangem uma organização.  <br/> |
|Floresta  <br/> |Os escopos de controle de mensagens abrangem uma floresta.  <br/> |
|Site  <br/> |Os escopos de controle de mensagens abrangem um site.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

