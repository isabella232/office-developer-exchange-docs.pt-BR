---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: O elemento UnknownEntries contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 68cb2518b895ca0a74e6b9ed649ee92b7502ab05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459416"
---
# <a name="unknownentries"></a>UnknownEntries

O elemento **UnknownEntries** contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 **ArrayOfUnknownEntriesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[UnknownEntry](unknownentry.md) <br/> |Representa uma única entrada de permissão desconhecida que não pode ser resolvida no Active Directory. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PermissionSet (PermissionSettype)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[PermissionSet (CalendarPermissionSetType)](permissionset-calendarpermissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta de calendário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

Você pode excluir entradas desconhecidas de uma pasta usando a operação UpdateFolder com o elemento [Setfolderfield](setfolderfield.md) . As entradas desconhecidas são excluídas quando você redefine o PermissionSet usando a opção setfolderfield da operação UpdateFolder. Os serviços Web do Exchange não oferecem suporte à exclusão de entradas individuais. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação UpdateFolder](updatefolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões no nível de pasta](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

