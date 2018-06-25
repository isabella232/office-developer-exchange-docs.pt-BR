---
title: IsDefault (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7358bb88-c441-4f2c-9647-c030e7303e8a
description: O elemento IsDefault indica se um documento local de compartilhamento padrão do usuário local de compartilhamento.
ms.openlocfilehash: 6e5e2958f4c9909968b976d73584b1060ee58dfa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823997"
---
# <a name="isdefault-soap"></a>IsDefault (SOAP)

O elemento **IsDefault** indica se um documento local de compartilhamento padrão do usuário local de compartilhamento. 
  
```XML
<IsDefault /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Representa informações de local e metadados para um local de compartilhamento de documentos.  <br/> |
   
## <a name="text-value"></a>Text value

O valor booliano do elemento **IsDefault** indica se o local de compartilhamento é o padrão do usuário local de compartilhamento. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos de Autodiscover XML SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

