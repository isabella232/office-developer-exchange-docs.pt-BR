---
title: GetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c96c2b4c-45cb-482a-a3bb-7a11a0fff43b
description: O elemento GetClientExtension representa uma solicitação para obter uma extensão de cliente.
ms.openlocfilehash: 9d3abb4572a5f74f24925d24a2fbbe8ded593731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752430"
---
# <a name="getclientextension"></a>GetClientExtension

O elemento **GetClientExtension** representa uma solicitação para obter uma extensão de cliente. 
  
```XML
<GetClientExtension>
   <RequestedExtensionIds/>
   <UserParameters/>
   <IsDebug/>
</GetClientExtension>
```

 ****
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[RequestedExtensionIds](requestedextensionids.md) | [Parâmetros_do_usuário](userparameters.md) | [IsDebug](isdebug.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

