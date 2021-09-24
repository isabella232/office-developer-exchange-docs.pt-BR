---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: O elemento UnknownEntries contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 9ada724abbecddf192b5f345c1800ac38a8b41aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514078"
---
# <a name="unknownentries"></a>UnknownEntries

O **elemento UnknownEntries** contém uma matriz de entradas de permissão desconhecidas que não podem ser resolvidas no serviço de diretório do Active Directory. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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
|[UnknownEntry](unknownentry.md) <br/> |Representa uma única entrada de permissão desconhecida que não pode ser resolvida em relação ao Active Directory. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[PermissionSet (CalendarPermissionSetType)](permissionset-calendarpermissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta de calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

Você pode excluir entradas desconhecidas de uma pasta usando a operação UpdateFolder com o [elemento SetFolderField.](setfolderfield.md) As entradas desconhecidas são excluídas quando você redefine o PermissionSet usando a opção SetFolderField da operação UpdateFolder. Exchange Os Serviços Web não suportam a exclusão de entradas individuais. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação UpdateFolder](updatefolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

