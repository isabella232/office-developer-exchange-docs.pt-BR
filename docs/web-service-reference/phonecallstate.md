---
title: Chamada do telefonema
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
description: O elemento callstate especifica o estado atual de uma chamada telefônica.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468527"
---
# <a name="phonecallstate"></a>Chamada do telefonema

O **elemento** callstate especifica o estado atual de uma chamada telefônica. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
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

A tabela a seguir lista os valores possíveis para o elemento de **chamada de chamada** . 
  
**Valores do elemento de chamada do telefonema**

|**Valor**|**Descrição**|
|:-----|:-----|
|Estado  <br/> |Estado de chamada inicial.  <br/> |
|Connecting  <br/> |O sistema está discando esta chamada.  <br/> |
|Alertado  <br/> |A chamada está em estado de alerta (o telefone está tocando).  <br/> |
|Conectado  <br/> |A chamada está no estado conectado.  <br/> |
|Disconnected  <br/> |A chamada é desconectada.  <br/> |
|Electrónico  <br/> |A chamada é de entrada.  <br/> |
|Transfer  <br/> |A chamada está sendo transferida para outro destino.  <br/> |
|Encaminhamento  <br/> |A chamada está sendo encaminhada para outro destino.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

