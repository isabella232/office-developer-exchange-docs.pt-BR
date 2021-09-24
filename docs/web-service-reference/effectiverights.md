---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: O elemento EffectiveRights contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura.
ms.openlocfilehash: a3207a9971065d3b69b6a0b7056fa8012425fd5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514708"
---
# <a name="effectiverights"></a>EffectiveRights

O **elemento EffectiveRights** contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura. 
  
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
|[CreateAssociated](createassociated.md) <br/> |Indica se um cliente pode criar uma tabela de conteúdo associada. Essa propriedade só é usada em objetos de pasta.  <br/> |
|[CreateContents](createcontents.md) <br/> |Indica se um cliente pode criar uma tabela de conteúdo. Essa propriedade só é usada em objetos de pasta.  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |Indica se um cliente pode criar uma tabela de hierarquia. Essa propriedade só é usada em objetos de pasta.  <br/> |
|[Delete](delete.md) <br/> |Indica se um cliente pode excluir uma pasta ou item.  <br/> |
|[Modificar](modify.md) <br/> |Indica se um cliente pode modificar uma pasta ou item.  <br/> |
|[Leitura](read.md) <br/> |Indica se um cliente pode ler uma pasta ou item.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indica se um item particular pode ser exibido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas em uma caixa de correio.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos em uma caixa de correio.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[Contato](contact.md) <br/> |Representa um Exchange de contato.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[Item](item.md) <br/> |Representa um item Exchange genérico.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma Exchange de email.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no Exchange store.  <br/> |
|[Item de postagem](postitem.md) <br/> |Representa um item post no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

**EffectiveRights** é suportado nas respostas GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy e SyncFolderItems. A **propriedade EffectiveRights** é exposta na forma **AllProperties** para pastas e itens. 
  
Essa **propriedade EffectiveRights** fornece acesso às mesmas informações fornecidas na propriedade **PR_ACCESS MAPI.** 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

