---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: O elemento RootFolder contém os resultados de uma pesquisa de uma única pasta raiz durante uma operação FindFolder.
ms.openlocfilehash: 582d4642bb4ecd2816beba6df863eb274762f804
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512272"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

O **elemento RootFolder** contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).
  
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
|IndexedPagingOffset  <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação ao usar um exibição de pajamento indexado.  <br/> |
|NumeratorOffset  <br/> |Representa o novo valor de numerador a ser usado para a próxima solicitação ao usar exibições de página fracionada.  <br/> |
|AbsoluteDenominator  <br/> |Representa o próximo denominador a ser usado para a próxima solicitação ao fazer pajamento fracional.  <br/> |
|IncludesLastItemInRange  <br/> |Indica se os resultados atuais contêm a última pasta na consulta, de forma que a pajamento posterior não seja necessária.  <br/> |
|TotalItemsInView  <br/> |Representa o número total de pastas que passam pela restrição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas encontradas usando a [operação FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação FindFolder.](findfolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindFolder](findfolder-operation.md)


[Localizar Pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

