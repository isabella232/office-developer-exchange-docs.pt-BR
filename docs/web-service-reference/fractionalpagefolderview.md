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
description: O elemento FractionalPageFolderView descreve onde o modo de exibição paginado é iniciado e o número máximo de pastas retornados em uma solicitação de FindFolder.
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752357"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

O elemento **FractionalPageFolderView** descreve onde o modo de exibição paginado é iniciado e o número máximo de pastas retornados em uma solicitação de [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a serem retornados na resposta [FindFolder](findfolder.md) . Este atributo é opcional.  <br/> |
|**Numerador** <br/> |Representa o numerador do deslocamento fracional desde o início do conjunto de resultados. Este atributo é necessário. O numerador deve ser igual ou menor que o denominador. Este atributo deve representar um valor integral que é igual ou maior do que zero. Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.  <br/> |
|**Denominador** <br/> |Representa o denominador do deslocamento fracional desde o início do número total de pastas no conjunto de resultados. Este atributo é necessário. Este atributo deve representar um valor inteiro maior que um. Para obter mais informações, consulte a seção comentários, mais adiante neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Coment�rios

O deslocamento do modo de exibição paginados desde o início do conjunto de pastas localizadas descrito por uma fração. A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciado. Por exemplo, se **numerador** é igual a quatro e **denominador** igual a cinco, a página de informações retornadas começa em uma entrada localizado quatro-quintas da maneira no conjunto de resultados. 
  
Se fração for avaliada como zero, o que indica o início do conjunto de resultados. Se fração for avaliada como um, que indica o fim do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto inicial da página, não quantos resultados no conjunto de resultados serão retornados. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

