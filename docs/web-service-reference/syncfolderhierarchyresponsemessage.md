---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: O elemento SyncFolderHierarchyResponseMessage contém o status e o resultado de uma única solicitação de operação SyncFolderHierarchy.
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837685"
---
# <a name="syncfolderhierarchyresponsemessage"></a>SyncFolderHierarchyResponseMessage

O elemento **SyncFolderHierarchyResponseMessage** contém o status e o resultado de uma única [operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) solicitação. 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) 
- [ResponseMessages](responsemessages.md)
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 **SyncFolderHierarchyResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta [SyncFolderHierarchy operação](syncfolderhierarchy-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:<br/>  <br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Sucesso** <br/> |Descreve uma solicitação que seja cumprida.  <br/> |
|**Warning** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados. <br/><br/>Estes são exemplos de fontes de avisos de:  <br/><br/>-O armazenamento do Exchange está offline durante o lote.  <br/>-Active Directory Domain Services (AD DS) está offline.  <br/>-Caixas de correio foram movidos.  <br/>-O banco de dados de mensagens (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/> |
|**Erro** <br/> | Descreve uma solicitação que não puder ser atendida. <br/><br/>Estes são exemplos de fontes de erros:  <br/><br/>-Inválido atributos e elementos  <br/>-Atributos ou elementos que estão fora do intervalo  <br/>-Uma marca desconhecida  <br/>-Um atributo ou elemento que não é válido no contexto  <br/>-Uma tentativa de acesso não autorizado por qualquer cliente  <br/>-Uma falha no servidor em resposta a uma chamada de cliente válida  <br/><br/>  Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |No momento não utilizados e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações de resposta de erro adicionais.  <br/> |
|[Estado de sincronização](syncstate-ex15websvcsotherref.md) <br/> |Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização.  <br/> |
|[IncludesLastFolderInRange](includeslastfolderinrange.md) <br/> |Indica se o último item para sincronizar foi incluído na resposta.  <br/> |
|[Alterações (hierarquia)](changes-hierarchy.md) <br/> |Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

