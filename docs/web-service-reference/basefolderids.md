---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: O elemento BaseFolderIds representa a coleção de pastas que serão mineradas para determinar o conteúdo de uma pasta de pesquisa.
ms.openlocfilehash: 3a108e6215c6a444117aa65c756352b9800f6948
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518943"
---
# <a name="basefolderids"></a>BaseFolderIds

O **elemento BaseFolderIds** representa a coleção de pastas que serão mineradas para determinar o conteúdo de uma pasta de pesquisa. 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica pastas do MicrosoftExchange Server 2007 que podem ser referenciadas pelo nome.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchParameters](searchparameters.md) <br/> |Representa os parâmetros que definem uma pasta de pesquisa.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento BaseFolderIds** deve conter pelo menos um [elemento FolderId](folderid.md) ou [DistinguishedFolderId.](distinguishedfolderid.md) 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

