---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: O elemento ConnectionFailureCause Especifica o motivo para uma desconexão de uma chamada telefônica.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751426"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

O elemento **ConnectionFailureCause** Especifica o motivo para uma desconexão de uma chamada telefônica. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Especifica as informações de estado de uma chamada telefônica.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **ConnectionFailureCause** . 
  
**Valores de elemento ConnectionFailureCause**

|**Valor**|**Descrição**|
|:-----|:-----|
|None  <br/> |Estado de chamada não for desconectado ou o motivo de desconexão não é conhecido.  <br/> |
|UserBusy  <br/> |A linha da parte chamada estava ocupada.  <br/> |
|NoAnswer  <br/> |A parte chamada não atendida.  <br/> |
|Unavailable  <br/> |O número da parte chamada não estava disponível.  <br/> |
|Outro  <br/> |Pega-tudo por outros motivos desconectar.  <br/> |
   
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

