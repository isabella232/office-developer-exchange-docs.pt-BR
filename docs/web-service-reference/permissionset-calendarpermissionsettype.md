---
title: PermissionSet (CalendarPermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: Elemento PermissionSet contém todas as permissões que estão configuradas para uma pasta de calendário.
ms.openlocfilehash: b2e642fd2ee8ded4d0d4c67509a5587f7b1efa8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824728"
---
# <a name="permissionset-calendarpermissionsettype"></a>PermissionSet (CalendarPermissionSetType)

Elemento **PermissionSet** contém todas as permissões que estão configuradas para uma pasta de calendário. 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **CalendarPermissonSetType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Contém uma matriz de permissões de calendário de uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Contém uma matriz de entradas de desconhecido que não pode ser resolvido em relação ao serviço de diretório do Active Directory. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Diferenças de versão

Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) . Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** . 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões de nível de pasta](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

