---
title: Permissões
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: O elemento Permissions contém a coleção de permissões para uma pasta.
ms.openlocfilehash: b8616cefdb8c453106753fb0788a6c7d6a0ded79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459213"
---
# <a name="permissions"></a>Permissions

O elemento **Permissions** contém a coleção de permissões para uma pasta. 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Permissão](permission.md) <br/> |Define o acesso que um representante tem a uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PermissionSet (PermissionSettype)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Diferenças de versão

Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) . Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** . 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões no nível de pasta](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

