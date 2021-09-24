---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: O elemento PhoneCallState especifica o estado atual de uma chamada telefônica.
ms.openlocfilehash: 8c0b8357b58826f18f05eb0fedc0865be1623c2b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528299"
---
# <a name="phonecallstate"></a>PhoneCallState

O **elemento PhoneCallState** especifica o estado atual de uma chamada telefônica. 
  
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
|[PhoneCallInformation](phonecallinformation.md) <br/> |Especifica as informações de estado para uma chamada telefônica.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento PhoneCallState.** 
  
**Valores do elemento PhoneCallState**

|**Valor**|**Descrição**|
|:-----|:-----|
|Idle  <br/> |Estado inicial da chamada.  <br/> |
|Connecting  <br/> |O sistema está discando essa chamada.  <br/> |
|Alertado  <br/> |A chamada está em estado de alerta (telefone está tocando).  <br/> |
|Conectado  <br/> |A chamada está no estado conectado.  <br/> |
|Disconnected  <br/> |A chamada está desconectada.  <br/> |
|Incoming  <br/> |A chamada é de entrada.  <br/> |
|Transferência  <br/> |A chamada está sendo transferida para outro destino.  <br/> |
|Encaminhamento  <br/> |A chamada está sendo encaminhada para outro destino.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório /ews/do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

