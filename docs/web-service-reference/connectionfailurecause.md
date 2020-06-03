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
description: O elemento ConnectionFailureCause especifica a razão para uma desconexão de uma chamada telefônica.
ms.openlocfilehash: 6385641eaee140a114906703232974d51d5ce344
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529445"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

O elemento **ConnectionFailureCause** especifica a razão para uma desconexão de uma chamada telefônica. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Especifica as informações de estado de uma chamada telefônica.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **ConnectionFailureCause** . 
  
**Valores do elemento ConnectionFailureCause**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |O estado de chamada não é desconectado ou o motivo da desconexão não é conhecido.  <br/> |
|Userbusy  <br/> |A linha do participante chamada estava ocupada.  <br/> |
|NOANSWER  <br/> |A parte chamada não respondeu.  <br/> |
|Indisponível  <br/> |O número da parte chamada não estava disponível.  <br/> |
|Outros  <br/> |Catch-tudo por outros motivos de desconexão.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

