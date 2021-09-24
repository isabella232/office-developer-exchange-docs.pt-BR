---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: O elemento CalendarPermissionLevel representa o nível de permissão que um usuário tem em uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e43b26f12fa65f47ca8377ecdd6c3abe2f6c5b71
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518831"
---
# <a name="calendarpermissionlevel"></a>CalendarPermissionLevel

O **elemento CalendarPermissionLevel** representa o nível de permissão que um usuário tem em uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 **CalendarPermissionLevelType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Define o acesso que um usuário tem a uma pasta Calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento CalendarPermissionLevel.** 
  
**Valores de texto do elemento CalendarPermissionLevel**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o usuário não tem permissões na pasta.  <br/> |
|Proprietário  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas. O usuário é o proprietário da pasta e o contato da pasta.  <br/> |
|PublishingEditor  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas.  <br/> |
|Editor  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta.  <br/> |
|PublishingAuthor  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta, editar e excluir somente itens que o usuário cria e criar subpastas.  <br/> |
|Autor  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta e editar e excluir somente itens que o usuário cria.  <br/> |
|NoneditingAuthor  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta e excluir somente itens que o usuário cria.  <br/> |
|Revisor  <br/> |Indica que o usuário pode ler todos os itens na pasta.  <br/> |
|Colaborador  <br/> |Indica que o usuário pode criar itens na pasta. O conteúdo da pasta não aparece.  <br/> |
|FreeBusyTimeOnly  <br/> |Indica que o usuário só pode exibir o tempo livre/ocupado no calendário.  <br/> |
|FreeBusyTimeAndSubjectAndLocation  <br/> |Indica que o usuário pode exibir o tempo livre/ocupado dentro do calendário e o assunto e o local dos compromissos.  <br/> |
|Personalizado  <br/> |Indica que o usuário tem permissões de acesso personalizadas na pasta.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

