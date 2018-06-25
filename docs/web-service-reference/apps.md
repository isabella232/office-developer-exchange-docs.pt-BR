---
title: Aplicativos
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: O elemento de aplicativos contém informações sobre todos os arquivos de manifesto de XML para os aplicativos instalados em uma caixa de correio.
ms.openlocfilehash: 81b0cb76b02fcc9145f6d70eff12a0a0ac0ad51f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751194"
---
# <a name="apps"></a>Aplicativos

O elemento de **aplicativos** contém informações sobre todos os arquivos de manifesto de XML para os aplicativos instalados em uma caixa de correio. 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[App](app.md)
  
### <a name="parent-elements"></a>Elementos pai

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Não aplicável  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [App](app.md)
- [GetAppManifestsResponse](getappmanifestsresponse.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

