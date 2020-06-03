---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: O elemento IncludeMimeContent especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta.
ms.openlocfilehash: 6198e4bef2dc59e6e56a8d3cbe463dad13e544e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457190"
---
# <a name="includemimecontent"></a>IncludeMimeContent

O elemento **IncludeMimeContent** especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta. 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .  <br/> <br/> A seguir está a expressão XPath para este elemento:  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[Shape](itemshape.md) <br/> | Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/> <br/> A seguir estão as expressões XPath para este elemento:<br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **true** ou **false**. O valor padrão é **false**. Este é um tipo de dados Boolean.
  
## <a name="remarks"></a>Comentários

Este elemento é opcional.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação demonstra como definir o elemento **IncludeMimeContent** . 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

O atributo ID do anexo é truncado para preservar a legibilidade.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

