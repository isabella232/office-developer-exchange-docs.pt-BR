---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: O elemento CopyToFolder Especifica o identificador da pasta esse email itens podem ser copiados para.
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751554"
---
# <a name="copytofolder"></a>CopyToFolder

O elemento **CopyToFolder** Especifica o identificador da pasta esse email itens podem ser copiados para. 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador de uma pasta de destino para um item movido ou copiada ou uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino nomeado para um item movido ou copiada ou uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ações](actions.md) <br/> |Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[MoveToFolder](movetofolder.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

