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
description: O elemento FolderName identifica uma única pasta personalizada gerenciada para adicionar uma caixa de correio.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752339"
---
# <a name="foldername"></a>FolderName

O elemento **FolderName** identifica uma única pasta personalizada gerenciada para adicionar uma caixa de correio. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[Nomes de pastas](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nomes de pastas](foldernames.md) <br/> |Contém uma matriz de nomeada pastas personalizadas gerenciadas para adicionar uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto representa um nome de pasta.
  
## <a name="remarks"></a>Comentários

Embora você possa usar os serviços Web do Exchange para adicionar pastas personalizadas gerenciadas a uma caixa de correio, você não pode usar a mesma tecnologia para acessar a lista de disponíveis pastas personalizadas gerenciadas. Você pode obter uma lista de pastas personalizadas gerenciadas usando um comando do Shell de gerenciamento do Exchange ou por meio de uma API que interage com o serviço de diretório do Active Directory. O nome da pasta é o nome do objeto do Active Directory correspondente.
  
Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas personalizadas gerenciadas. Use a [operação DeleteFolder](deletefolder-operation.md) para excluir o pastas personalizadas gerenciadas. 
  
É importante observar que o **nome da pasta** é o nome de uma pasta de personalizada gerenciada existente na organização. Uma tentativa de adicionar uma pasta que não esteja na organização resultará em uma resposta de erro. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindFolder](findfolder-operation.md)


[Localizando pastas](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Adicionando pastas gerenciadas](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

