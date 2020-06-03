---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: O elemento EffectiveRights contém os direitos do cliente com base nas configurações de permissão para o item ou pasta. Este elemento é somente leitura.
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459241"
---
# <a name="effectiverights"></a>EffectiveRights

O elemento **EffectiveRights** contém os direitos do cliente com base nas configurações de permissão para o item ou pasta. Este elemento é somente leitura. 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 **EffectiveRightsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Createassociado](createassociated.md) <br/> |Indica se um cliente pode criar uma tabela de conteúdo associado. Esta propriedade só é usada em objetos Folder.  <br/> |
|[Createcontents](createcontents.md) <br/> |Indica se um cliente pode criar uma tabela de conteúdo. Esta propriedade só é usada em objetos Folder.  <br/> |
|[Createhierarchy](createhierarchy.md) <br/> |Indica se um cliente pode criar uma tabela de hierarquia. Esta propriedade só é usada em objetos Folder.  <br/> |
|[Delete](delete.md) <br/> |Indica se um cliente pode excluir uma pasta ou item.  <br/> |
|[Modificar](modify.md) <br/> |Indica se um cliente pode modificar uma pasta ou item.  <br/> |
|[Leitura](read.md) <br/> |Indica se um cliente pode ler uma pasta ou item.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indica se um item particular pode ser exibido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta tarefas em uma caixa de correio.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta contatos em uma caixa de correio.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item de postagem no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

**EffectiveRights** é suportado nas respostas GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy e SyncFolderItems. A propriedade **EffectiveRights** é exposta na forma de **Propriedades** para pastas e itens. 
  
Esta propriedade **EffectiveRights** fornece acesso às mesmas informações fornecidas na propriedade **PR_ACCESS MAPI** . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Definindo permissões no nível de pasta](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

