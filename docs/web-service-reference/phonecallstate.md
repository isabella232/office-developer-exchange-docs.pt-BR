---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: O elemento PhoneCallState Especifica o estado atual de uma chamada telefônica.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824761"
---
# <a name="phonecallstate"></a>PhoneCallState

O elemento **PhoneCallState** Especifica o estado atual de uma chamada telefônica. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
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

A tabela a seguir lista os valores possíveis para o elemento **PhoneCallState** . 
  
**Valores de elemento PhoneCallState**

|**Valor**|**Descrição**|
|:-----|:-----|
|Ocioso  <br/> |Estado inicial de chamada.  <br/> |
|Connecting  <br/> |O sistema está discando essa chamada.  <br/> |
|Alertado  <br/> |A chamada está no estado de alerta (telefone está tocando).  <br/> |
|Connected  <br/> |A chamada está no estado conectado.  <br/> |
|Disconnected  <br/> |A chamada é desconectada.  <br/> |
|Entrada  <br/> |A chamada é entrada.  <br/> |
|Transferindo  <br/> |A chamada está sendo transferida para outro destino.  <br/> |
|Encaminhamento  <br/> |A chamada está sendo encaminhada para outro destino.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório /ews/ do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

