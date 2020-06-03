---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: O elemento RootFolder contém os resultados de uma pesquisa de uma única pasta raiz durante uma operação FindFolder.
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457134"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

O elemento **RootFolder** contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação ao usar um modo de exibição de paginação indexado.  <br/> |
|NumeratorOffset  <br/> |Representa o novo valor do numerador a ser usado para a próxima solicitação ao usar as exibições de página fracionada.  <br/> |
|AbsoluteDenominator  <br/> |Representa o próximo denominador a ser usado para a próxima solicitação ao fazer paginação fracionária.  <br/> |
|IncludesLastItemInRange  <br/> |Indica se os resultados atuais contêm a última pasta na consulta, de modo que a paginação adicional não será necessária.  <br/> |
|TotalItemsInView  <br/> |Representa o número total de pastas que passam a restrição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas encontradas usando a [operação FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação FindFolder](findfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

