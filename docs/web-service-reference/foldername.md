---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: O elemento FolderName identifica uma única pasta personalizada gerenciada para adicionar a uma caixa de correio.
ms.openlocfilehash: 1bb63e50c06e81337d1142a6624213fb2db12457
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461349"
---
# <a name="foldername"></a>FolderName

O elemento **foldername** identifica uma única pasta personalizada gerenciada para adicionar a uma caixa de correio. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Contém uma matriz de pastas personalizadas gerenciadas e nomeadas para adicionar a uma caixa de correio.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor de texto representa um nome de pasta.
  
## <a name="remarks"></a>Comentários

Embora você possa usar os serviços Web do Exchange para adicionar pastas personalizadas gerenciadas a uma caixa de correio, não é possível usar a mesma tecnologia para acessar a lista de pastas personalizadas gerenciadas disponíveis. Você pode obter uma lista de pastas personalizadas gerenciadas usando um comando do Shell de gerenciamento do Exchange ou usando uma API que faz interface com o serviço de diretório do Active Directory. O nome da pasta é o nome do objeto do Active Directory correspondente.
  
Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas personalizadas gerenciadas. Use a [operação DeleteFolder](deletefolder-operation.md) para excluir pastas personalizadas gerenciadas. 
  
É importante observar que **foldername** é o nome de uma pasta personalizada gerenciada existente na organização. Uma tentativa de adicionar uma pasta que não esteja na organização resultará em uma resposta de erro. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

