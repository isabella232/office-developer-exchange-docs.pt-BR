---
title: IncludesLastItemInRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludesLastItemInRange
api_type:
- schema
ms.assetid: e7d6c7d3-548e-48b0-a313-bfef81e4832a
description: O elemento IncludesLastItemInRange indica se o último item para sincronizar foi incluído na resposta.
ms.openlocfilehash: b4786c5aa81e9b4fee98e7ed4238215ff327443e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823906"
---
# <a name="includeslastiteminrange"></a>IncludesLastItemInRange

O elemento **IncludesLastItemInRange** indica se o último item para sincronizar foi incluído na resposta. 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[IncludesLastItemInRange](includeslastiteminrange.md)
  
```xml
<IncludesLastItemInRange/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um valor booleano.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação SyncFolderItems](syncfolderitems-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

