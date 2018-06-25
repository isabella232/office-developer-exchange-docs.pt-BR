---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: O elemento de CreateFolder define uma solicitação para criar uma pasta no repositório do Exchange.
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751579"
---
# <a name="createfolder"></a>CreateFolder

O elemento de **CreateFolder** define uma solicitação para criar uma pasta no repositório do Exchange. 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 **CreateFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |O elemento que identifica o local onde a nova pasta é criada.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |O elemento que contém todas as pastas para criar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação CreateFolder](createfolder-operation.md)


[Criação de pastas (serviços Web do Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

