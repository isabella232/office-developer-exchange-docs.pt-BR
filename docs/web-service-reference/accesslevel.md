---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: O elemento AccessLevel especifica o nível de acesso para uma reunião online.
ms.openlocfilehash: 3c1375ef37ea666c6c4fafce7daa46ae0d0a2696
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462336"
---
# <a name="accesslevel"></a>AccessLevel

O elemento **AccessLevel** especifica o nível de acesso para uma reunião online. 
  
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

A tabela a seguir lista os valores de texto para o elemento **AccessLevel** . 
  
**Valores de texto do elemento AccessLevel**

|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |O nível de acesso é aberto para todos.  <br/> |
|Interno  <br/> |O nível de acesso é somente interno.  <br/> |
|Convidar  <br/> |O nível de acesso é somente participantes convidados.  <br/> |
|Bloqueado  <br/> |O nível de acesso está bloqueado.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2013.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

