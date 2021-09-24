---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: O elemento FractionalPageFolderView descreve onde o exibição paged é iniciado e o número máximo de pastas retornadas em uma solicitação FindFolder.
ms.openlocfilehash: b3d4bd63f94c2db7761dabfad1e32558ceb30be5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530250"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

O **elemento FractionalPageFolderView** descreve onde o exibição paged é iniciado e o número máximo de pastas retornadas em uma [solicitação FindFolder.](findfolder.md) 
  
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
|**MaxEntriesReturned** <br/> |Identifica o número máximo de resultados a ser retornado na [resposta FindFolder.](findfolder.md) Esse atributo é opcional.  <br/> |
|**Numerador** <br/> |Representa o numerador do deslocamento fracional desde o início do conjunto de resultados. Esse atributo é necessário. O numerador deve ser igual ou menor que o denominador. Esse atributo deve representar um valor integral igual ou maior que zero. Para obter mais informações, consulte Comentários posteriormente neste tópico.  <br/> |
|**Denominador** <br/> |Representa o denominador do deslocamento fracional desde o início do número total de pastas no conjunto de resultados. Esse atributo é necessário. Esse atributo deve representar um valor integral maior do que um. Para obter mais informações, consulte Comentários posteriormente neste tópico.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Comentários

O deslocamento de exibição pagedo do início do conjunto de pastas encontradas é descrito por uma fração. A fração, que é definida pelos **atributos Numerador** e **Denominador,** descreve onde a página de informações é iniciada. Por exemplo, se **Numerador** for igual a quatro e **Denominador** for igual a cinco, a página de informações retornadas começará em uma entrada localizada quatro quintos do caminho para o conjunto de resultados. 
  
Se a fração for avaliada como zero, isso indicará o início do conjunto de resultados. Se a fração for avaliada como um, isso indicará o final do conjunto de resultados.
  
> [!NOTE]
> A fração representa o ponto inicial da página, e não quantos resultados no conjunto de resultados serão retornados. 
  
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


[Localizar Pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

