---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: O elemento de DeleteFolder define uma solicitação para excluir pastas de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751746"
---
# <a name="deletefolder"></a>DeleteFolder

O elemento de **DeleteFolder** define uma solicitação para excluir pastas de uma caixa de correio no armazenamento do Exchange. 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**DeleteType** <br/> |Descreve como uma pasta é excluída. Este atributo é necessário.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |Uma pasta é removida permanentemente do repositório.  <br/> |
|SoftDelete  <br/> |Uma pasta é movida para o dumpster se o dumpster está habilitado.  <br/> |
|MoveToDeletedItems  <br/> |Uma pasta é movida para a pasta Itens excluídos.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para excluir.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que no momento em uma chamada de serviço da Web for concluído, o banco de dados tiver movido o item para a pasta Itens excluídos ou removido permanentemente o item do banco de dados do Exchange. Esse comportamento é o mesmo para MicrosoftExchange Server 2007 e o Exchange Server 2010. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação DeleteFolder](deletefolder-operation.md)

