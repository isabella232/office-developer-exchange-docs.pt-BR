---
title: Grupos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: O elemento Groups contém uma coleção de grupos que são encontrados com os critérios de pesquisa e agregação identificados na solicitação de operação FindItem.
ms.openlocfilehash: f47ab4111137d2e5d98fcc6dcf40fadc073b7af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539679"
---
# <a name="groups"></a>Grupos

O **elemento Groups** contém uma coleção de grupos que são encontrados com os critérios de pesquisa e agregação identificados na solicitação de operação [FindItem.](finditem-operation.md) 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 **ArrayOfGroupedItemsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |Representa uma coleção de itens que são o resultado de uma chamada de operação [FindItem](finditem-operation.md) agrupada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem.](finditem-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

Uma [instância GroupedItems](groupeditems.md) ocorrerá para cada grupo distinto dentro do resultado. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindItem](finditem-operation.md)


[Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

