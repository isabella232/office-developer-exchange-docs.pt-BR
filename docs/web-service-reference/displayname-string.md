---
title: DisplayName (string)
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
description: O elemento de DisplayName define o nome de exibição de uma pasta, contatos, lista de distribuição, usuário delegado, local ou regra.
ms.openlocfilehash: 53f4e083d9e6617206e383d4408e08ed7ea0fe08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751874"
---
# <a name="displayname-string"></a>DisplayName (string)

O elemento de **DisplayName** define o nome de exibição de uma pasta, contatos, lista de distribuição, usuário delegado, local ou regra. 
  
```XML
<DisplayName/>
```

 **String**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contato em uma caixa de correio.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma regra de caixa de correio do usuário.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefa em uma caixa de correio.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa o nome de exibição.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="example"></a>Exemplo

O exemplo a seguir mostra como criar uma nova pasta e para definir o DisplayName da pasta a "TestFolder".
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

