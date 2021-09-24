---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: O elemento PermissionSet contém todas as permissões configuradas para uma pasta de calendário.
ms.openlocfilehash: 26351be8fd9fbe56ea5abb2dd346cb9c9458c463
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539148"
---
# <a name="permissionset-calendarpermissionsettype"></a>PermissionSet (CalendarPermissionSetType)

O **elemento PermissionSet** contém todas as permissões configuradas para uma pasta de calendário. 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **CalendarPermissonSetType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Contém uma matriz de permissões de calendário para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Contém uma matriz de entradas desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Esse elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Diferenças de versão

Para aplicativos destinados Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o [elemento BaseShape](baseshape.md) tem um valor **allProperties** no [GetFolder](getfolder-operation.md) solicitação de operação. Para recuperar permissões de pasta, adicione o [elemento PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao [elemento AdditionalProperties](additionalproperties.md) na **solicitação GetFolder.** 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

