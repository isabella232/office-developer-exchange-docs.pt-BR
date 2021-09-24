---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: O elemento EmptyFolder define uma solicitação para esvaziar uma pasta em uma caixa de correio no Exchange store. Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada.
ms.openlocfilehash: c1b0e953f677c1fe5ae0958b35f85f3f5c4fb973
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519671"
---
# <a name="emptyfolder"></a>EmptyFolder

O **elemento EmptyFolder** define uma solicitação para esvaziar uma pasta em uma caixa de correio no Exchange store. Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada. 
  
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
|**DeleteSubFolders** <br/> |Especifica se subpastas devem ser excluídas. Esse atributo é necessário.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |As mensagens e pastas são removidas permanentemente do armazenamento.  <br/> |
|SoftDelete  <br/> |Uma mensagem e pastas são movidas para o dumpster se a lixeira estiver habilitada.  <br/> |
|MoveToDeletedItems  <br/> |Uma mensagem e pastas são movidas para a pasta Itens Excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas a ser excluídos.  <br/> |
   
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

