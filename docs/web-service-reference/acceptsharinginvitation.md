---
title: AcceptSharingInvitation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AcceptSharingInvitation
api_type:
- schema
ms.assetid: 3c2a47d6-490d-425b-8893-089a4f8882cd
description: O elemento AcceptSharingInvitation é usado para aceitar um convite que permite o acesso aos dados de contatos ou de calendário de outro usuário.
ms.openlocfilehash: 06439739e6cc544d5039ac9d18e0452b1d42a0ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752191"
---
# <a name="acceptsharinginvitation"></a>AcceptSharingInvitation

O elemento **AcceptSharingInvitation** é usado para aceitar um convite que permite o acesso aos dados de contatos ou de calendário de outro usuário. 
  
```xml
<AcceptSharingInvitation>
   <ReferenceItemId/>
</AcceptSharingInvitation>
```

 **AcceptSharingInvitationType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Identifica o item ao qual se refere no objeto response.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.  <br/> |
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
   
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

- [CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

