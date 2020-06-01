---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: O elemento ContactsView define uma pesquisa para itens de contato com base em nomes de exibição em ordem alfabética.
ms.openlocfilehash: 23c3fe13c44cdd0e5a054ecb3378bc3d633e55aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463815"
---
# <a name="contactsview"></a>ContactsView

O elemento **ContactsView** define uma pesquisa para itens de contato com base em nomes de exibição em ordem alfabética. 
  
[FindItem](finditem.md)
  
[ContactsView](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

**ContactsViewType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Descreve o número máximo de resultados a serem retornados na resposta [FindItem](finditem.md) .  <br/> |
|**Initialname** <br/> |Define o primeiro nome na lista de contatos a ser retornado na resposta. Se o nome inicial especificado não estiver na lista de contatos, o próximo nome da ordem alfabética definido pelo contexto cultural será retornado, exceto se o próximo nome vier após o **finalname**. Se o atributo **inicialname** for omitido, a resposta conterá uma lista de contatos que inicia com o primeiro nome na lista de contatos. Esse atributo é opcional.  <br/> |
|**Finalname** <br/> |Define o último nome na lista de contatos para retornar na resposta. Se o atributo **finalname** for omitido, a resposta conterá todos os contatos subsequentes na ordem de classificação especificada. Se o nome final especificado não estiver na lista de contatos, o nome da próxima ordem alfabética definido pelo contexto cultural será excluído.  <br/><br/>Por exemplo, se Finalname = "Name", mas Name não estiver na lista de contatos, os contatos com nomes de exibição de Nome1 ou NAME não serão incluídos.  <br/><br/>Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.<br/><br/> A seguir está a expressão XPath para este elemento:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação demonstra como localizar os primeiros três contatos começando com o contato com o nome de exibição de Kelly Rollin.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindItem](finditem-operation.md)
- [Localizar itens](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

