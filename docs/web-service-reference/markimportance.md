---
title: MarkImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkImportance
api_type:
- schema
ms.assetid: 32b8b08f-65e9-4764-b40a-63245551f4a3
description: O elemento MarkImportance Especifica a importância que deve ser marcada em mensagens.
ms.openlocfilehash: 32b1fa63ef47327e7d3af717ed9f452e43b16380
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824356"
---
# <a name="markimportance"></a>MarkImportance

O elemento **MarkImportance** Especifica a importância que deve ser marcada em mensagens. 
  
```XML
<MarkImportance/>
```

 **ImportanceChoicesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ações](actions.md) <br/> |Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto para esse elemento é restrito a um dos valores de cadeia de caracteres a seguir:
  
- Baixa
    
- Normal
    
- Alta
    
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

