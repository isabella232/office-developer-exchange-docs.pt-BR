---
title: MustDisplayComment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MustDisplayComment
api_type:
- schema
ms.assetid: 11d4d3c3-4652-4ed4-9b29-a0b5f85b82b7
description: O elemento MustDisplayComment indica se o comentário de pasta gerenciada deve ser exibido.
ms.openlocfilehash: 9a7e6a88b77ff9f1fd82507b8320898c195cd190
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824502"
---
# <a name="mustdisplaycomment"></a>MustDisplayComment

O elemento **MustDisplayComment** indica se o comentário de pasta gerenciada deve ser exibido. 
  
```xml
<MustDisplayComment/>
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
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa um valor booleano. Um valor **true** indica que o comentário deve ser exibido; um valor **false** indica que o comentário não tem a ser exibido. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

