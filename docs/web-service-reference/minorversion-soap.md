---
title: MinorVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef4e181-7324-4c88-94a9-1cffefc8c008
description: O elemento MinorVersion representa o número da versão secundária do servidor.
ms.openlocfilehash: 79e617e65e7cecffa1b8ca7ccfe9ac799bb475b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467750"
---
# <a name="minorversion-soap"></a>MinorVersion (SOAP)

O elemento **MinorVersion** representa o número da versão secundária do servidor. 
  
```XML
<MinorVersion/>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ServerVersionInfo (SOAP)](serverversioninfo-soap.md) <br/> |Contém a versão do servidor que processou a solicitação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor inteiro que representa o número da versão secundária do servidor que processou a solicitação.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

