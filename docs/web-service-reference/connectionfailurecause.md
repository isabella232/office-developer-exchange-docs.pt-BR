---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: O elemento ConnectionFailureCause especifica o motivo de uma desconexão de uma chamada telefônica.
ms.openlocfilehash: de2f06ae89577b0141b8555f98dba1671a228d45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543531"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

O **elemento ConnectionFailureCause** especifica o motivo de uma desconexão de uma chamada telefônica. 
  
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
|[PhoneCallInformation](phonecallinformation.md) <br/> |Especifica as informações de estado para uma chamada telefônica.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento ConnectionFailureCause.** 
  
**Valores do elemento ConnectionFailureCause**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |O estado da chamada não está desconectado ou o motivo da desconexão não é conhecido.  <br/> |
|UserBusy  <br/> |A linha de terceiros chamada estava ocupada.  <br/> |
|NoAnswer  <br/> |A parte chamada não atendeu.  <br/> |
|Indisponível  <br/> |O número da parte chamada não estava disponível.  <br/> |
|Outros  <br/> |Catch-all por outros motivos de desconexão.  <br/> |
   
## <a name="remarks"></a>Comentários

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

