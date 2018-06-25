---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: O elemento AdditionalProperties identifica propriedades adicionais para uso em GetItem, UpdateItem, CreateItem, FindItem ou FindFolder solicitações.
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751056"
---
# <a name="additionalproperties"></a>AdditionalProperties

O elemento **AdditionalProperties** identifica propriedades adicionais para uso em [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou [FindFolder](findfolder.md) solicitações. 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades estendidas de MAPI para obter, definir ou criar.  <br/> |
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica as propriedades de dicionário frequentemente referenciado pelo URI.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifica as propriedades de pasta para incluir em uma resposta [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [SyncFolderHierarchy](syncfolderhierarchy.md) .<br/><br/>  A seguir estão as expressões XPath para esse elemento:<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta [GetItem](getitem.md), [FindItem](finditem.md)ou [SyncFolderItems](syncfolderitems.md) .<br/><br/>  A seguir estão as expressões XPath para esse elemento:<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifica as propriedades de item estendido adicional para retornar em resposta a uma solicitação de [GetItem](getitem.md) .<br/><br/> Este é a expressão XPath para esse elemento:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>Comentários

Não todos os elementos filhos podem ser usados com [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)ou solicitações [FindFolder](findfolder.md) . A propriedade deve ser aplica à pasta ou item é acessado. Use propriedades estendidas para acessar outras propriedades. Se a propriedade não existe para um determinado item, nenhum elemento correspondente será emitido para o XML resultante. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
Esse elemento é opcional.
  
## <a name="example"></a>Exemplo

O exemplo de solicitação a seguir mostra como obter um assunto do item usando o elemento **AdditionalProperties** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

