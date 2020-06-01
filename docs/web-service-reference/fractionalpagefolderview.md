---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: O elemento FractionalPageFolderView descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463066"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

O elemento **FractionalPageFolderView** descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a serem retornados na resposta [FindFolder](findfolder.md) . Esse atributo é opcional.  <br/> |
|**Numera** <br/> |Representa o numerador do deslocamento fracionado do início do conjunto de resultados. Esse atributo é necessário. O numerador deve ser igual ou menor que o denominador. Este atributo deve representar um valor inteiro igual ou maior que zero. Para obter mais informações, consulte comentários mais adiante neste tópico.  <br/> |
|**Denominado** <br/> |Representa o denominador do deslocamento fracionado desde o início do número total de pastas no conjunto de resultados. Esse atributo é necessário. Este atributo deve representar um valor integral maior que um. Para obter mais informações, consulte comentários mais adiante neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Comentários

O deslocamento de modo de exibição paginado desde o início do conjunto de pastas encontradas é descrito por uma fração. A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciada. Por exemplo, se o **numerador** for igual a quatro e o **denominador** for igual a cinco, a página de informações retornadas será iniciada em uma entrada localizada em quatro cinco quinto da forma no conjunto de resultados. 
  
Se a fração for avaliada como zero, isso indica o início do conjunto de resultados. Se a fração for avaliada como um, isso indica o final do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto de início da página, não quantos resultados serão retornados no conjunto de resultados. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

