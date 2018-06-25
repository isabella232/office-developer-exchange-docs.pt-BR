---
title: Excluir
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: O elemento de excluir indica se um cliente pode excluir uma pasta ou item.
ms.openlocfilehash: 8a00a24ea63fa564ecefb96a5caed3a9199690eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751727"
---
# <a name="delete"></a>Excluir

O elemento **Excluir** indica se um cliente pode excluir uma pasta ou item. 
  
```XML
<Delete>true or false</Delete>
```

**boolean**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.  <br/> |
|[Ações](actions.md) <br/> |Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** indica que um cliente pode excluir um item ou pasta. Um valor **false** indica que um cliente não é possível excluir um item ou pasta. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Definindo permissões de nível de pasta](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

