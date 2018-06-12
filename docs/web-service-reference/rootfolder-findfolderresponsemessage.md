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
description: O elemento RootFolder contém os resultados de uma pesquisa de uma pasta raiz única durante uma operação FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825253"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

O elemento **RootFolder** contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindFolder](findfolder-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |Representa o próximo índice que deve ser usado para a próxima solicitação ao usar o modo de exibição indexada paginação.  <br/> |
|NumeratorOffset  <br/> |Representa o novo valor numerador usada para a próxima solicitação quando usar exibições de página fracionais.  <br/> |
|AbsoluteDenominator  <br/> |Representa o denominador próximo a ser usado para a próxima solicitação ao fazer a paginação fracional.  <br/> |
|IncludesLastItemInRange  <br/> |Indica se os resultados atuais contêm a última pasta na consulta, de forma que não seja necessário paginação ainda mais.  <br/> |
|TotalItemsInView  <br/> |Representa o número total de pastas que passam a restrição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz das pastas encontrado usando a [operação FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação FindFolder](findfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

