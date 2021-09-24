---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: O elemento AdditionalProperties identifica propriedades adicionais para uso em solicitações GetItem, UpdateItem, CreateItem, FindItem ou FindFolder.
ms.openlocfilehash: 9a6fb98e9a88b1e40bd83559b1836d4122f0f125
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522198"
---
# <a name="additionalproperties"></a>AdditionalProperties

O **elemento AdditionalProperties** identifica propriedades adicionais para uso em solicitações [GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)ou [FindFolder.](findfolder.md) 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI estendidas para obter, definir ou criar.  <br/> |
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica as propriedades de dicionário referenciadas com frequência pelo URI.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifica as propriedades da pasta a incluir em uma [resposta GetFolder,](getfolder.md) [FindFolder](findfolder.md)ou [SyncFolderHierarchy.](syncfolderhierarchy.md)<br/><br/>  Veja a seguir as expressões XPath para este elemento:<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta [GetItem,](getitem.md) [FindItem](finditem.md)ou [SyncFolderItems.](syncfolderitems.md)<br/><br/>  Veja a seguir as expressões XPath para este elemento:<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifica propriedades de item estendidas adicionais para retornar em uma resposta a uma [solicitação GetItem.](getitem.md)<br/><br/> Veja a seguir a expressão XPath para este elemento:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>Comentários

Nem todos os elementos filho podem ser usados com solicitações [GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)ou [FindFolder.](findfolder.md) A propriedade deve ser aplicável à pasta ou item acessado. Use propriedades estendidas para acessar outras propriedades. Se a propriedade não existir para um determinado item, nenhum elemento correspondente será emitido no XML resultante. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
Esse elemento é opcional.
  
## <a name="example"></a>Exemplo

O exemplo de solicitação a seguir mostra como obter um assunto de item usando o **elemento AdditionalProperties.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

