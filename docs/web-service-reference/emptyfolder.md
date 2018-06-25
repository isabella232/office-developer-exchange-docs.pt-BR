---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: O elemento de EmptyFolder define uma solicitação para esvaziar a uma pasta em uma caixa de correio no armazenamento do Exchange. Opcionalmente, subpastas também podem ser excluídas quando a pasta será esvaziada.
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752037"
---
# <a name="emptyfolder"></a>EmptyFolder

O elemento de **EmptyFolder** define uma solicitação para esvaziar a uma pasta em uma caixa de correio no armazenamento do Exchange. Opcionalmente, subpastas também podem ser excluídas quando a pasta será esvaziada. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**DeleteType** <br/> |Especifica como uma pasta é esvaziada. Este atributo é necessário.  <br/> |
|**DeleteSubFolders** <br/> |Especifica se as subpastas estão a ser excluído. Este atributo é necessário.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |Uma mensagens e pastas são removidas permanentemente do repositório.  <br/> |
|SoftDelete  <br/> |Uma mensagens e pastas são movidas para o dumpster se o dumpster está habilitado.  <br/> |
|MoveToDeletedItems  <br/> |Uma mensagens e pastas são movidas para a pasta Itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para excluir.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação EmptyFolder](emptyfolder-operation.md)

