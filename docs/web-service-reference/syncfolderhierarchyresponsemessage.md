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
description: O elemento SyncFolderHierarchyResponseMessage contém o status e o resultado de uma única solicitação de operação de SyncFolderHierarchy.
ms.openlocfilehash: fda0a37178f89ba0fd5ef860f8b009f335a11391
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465342"
---
# <a name="syncfolderhierarchyresponsemessage"></a>SyncFolderHierarchyResponseMessage

O elemento **SyncFolderHierarchyResponseMessage** contém o status e o resultado de uma única solicitação de [operação de SyncFolderHierarchy](syncfolderhierarchy-operation.md) . 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ResponseClass** <br/> | Descreve o status de uma resposta de [operação do SyncFolderHierarchy](syncfolderhierarchy-operation.md) . <br/><br/>Os seguintes valores são válidos para este atributo:<br/>  <br/>-Êxito  <br/>-Aviso  <br/>-Erro  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valores de atributo ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|**Success** <br/> |Descreve uma solicitação que é atendida.  <br/> |
|**Aviso** <br/> | Descreve uma solicitação que não foi processada. Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes. <br/><br/>A seguir estão exemplos de fontes de avisos:  <br/><br/>– O repositório do Exchange está offline durante o lote.  <br/>– Os serviços de domínio do Active Directory (AD DS) estão offline.  <br/>-As caixas de correio foram movidas.  <br/>– O banco de dados de mensagens (MDB) está offline.  <br/>-Uma senha expirou.  <br/>-Uma cota foi excedida.  <br/> |
|**Error** <br/> | Descreve uma solicitação que não pode ser atendida. <br/><br/>A seguir estão exemplos de fontes de erros:  <br/><br/>-Atributos ou elementos inválidos  <br/>-Atributos ou elementos que estão fora do intervalo  <br/>-Uma marca desconhecida  <br/>-Um atributo ou elemento que não é válido no contexto  <br/>– Uma tentativa de acesso não autorizado por qualquer cliente  <br/>-Uma falha do servidor em resposta a uma chamada válida do lado do cliente  <br/><br/>  As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece um código de erro que identifica o erro específico que a solicitação encontrou.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Não utilizado no momento e está reservado para uso futuro. Ele contém um valor de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contém uma forma codificada em base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida. Isso é usado para identificar o estado de sincronização.  <br/> |
|[IncludesLastFolderInRange](includeslastfolderinrange.md) <br/> |Indica se o último item a ser sincronizado foi incluído na resposta.  <br/> |
|[Alterações (hierarquia)](changes-hierarchy.md) <br/> |Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

