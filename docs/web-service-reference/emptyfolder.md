---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: O elemento EmptyFolder define uma solicitação para esvaziar uma pasta em uma caixa de correio no repositório do Exchange. Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457274"
---
# <a name="emptyfolder"></a>EmptyFolder

O elemento **EmptyFolder** define uma solicitação para esvaziar uma pasta em uma caixa de correio no repositório do Exchange. Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**DeleteType** <br/> |Especifica como uma pasta é esvaziada. Esse atributo é necessário.  <br/> |
|**DeleteSubFolders** <br/> |Especifica se as subpastas devem ser excluídas. Esse atributo é necessário.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |As mensagens e pastas são removidas permanentemente da loja.  <br/> |
|SoftDelete  <br/> |As mensagens e pastas serão movidas para o dumpster se o dumpster estiver habilitado.  <br/> |
|MoveToDeletedItems  <br/> |As mensagens e pastas são movidas para a pasta itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas a serem excluídas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação EmptyFolder](emptyfolder-operation.md)

