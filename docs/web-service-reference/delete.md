---
title: Excluir
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: O elemento Delete indica se um cliente pode excluir uma pasta ou item.
ms.openlocfilehash: e1ecbfbcb11be04e39dc8353140653e6b5ca1c3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542488"
---
# <a name="delete"></a>Excluir

O **elemento Delete** indica se um cliente pode excluir uma pasta ou item. 
  
```XML
<Delete>true or false</Delete>
```

**boolean**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão do item ou pasta.  <br/> |
|[Actions](actions.md) <br/> |Representa o conjunto de ações que estão disponíveis para serem tomadas em uma mensagem quando as condições são atendidas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que um cliente pode excluir um item ou pasta. Um valor false indica **que** um cliente não pode excluir um item ou pasta. 
  
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
- [Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

