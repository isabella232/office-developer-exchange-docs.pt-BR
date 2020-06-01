---
title: DisplayName (cadeia de caracteres)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: O elemento DisplayName define o nome de exibição de uma pasta, contato, lista de distribuição, usuário delegado, local ou regra.
ms.openlocfilehash: 9b566ec1938ec206e45cddf9c7f00083af2d8a9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463613"
---
# <a name="displayname-string"></a>DisplayName (cadeia de caracteres)

O elemento **DisplayName** define o nome de exibição de uma pasta, contato, lista de distribuição, usuário delegado, local ou regra. 
  
```XML
<DisplayName/>
```

 **String**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos em uma caixa de correio.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma regra na caixa de correio de um usuário.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas em uma caixa de correio.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso à pasta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa o nome de exibição será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

Este exemplo a seguir mostra como criar uma nova pasta e definir o DisplayName da pasta como "TestFolder".
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

