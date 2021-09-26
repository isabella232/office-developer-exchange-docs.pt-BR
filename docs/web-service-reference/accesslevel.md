---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: O elemento AccessLevel especifica o nível de acesso de uma reunião online.
ms.openlocfilehash: f1c85579affe7d1142b22a890808bceeb8f82d38
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544413"
---
# <a name="accesslevel"></a>AccessLevel

O **elemento AccessLevel** especifica o nível de acesso de uma reunião online. 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |Especifica as configurações para reuniões online.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores de texto do **elemento AccessLevel.** 
  
**Valores de texto do elemento AccessLevel**

|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |O nível de acesso está aberto a todos.  <br/> |
|Interno  <br/> |O nível de acesso é somente interno.  <br/> |
|Convidado  <br/> |O nível de acesso é somente participantes convidados.  <br/> |
|Bloqueado  <br/> |O nível de acesso está bloqueado.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2013.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

