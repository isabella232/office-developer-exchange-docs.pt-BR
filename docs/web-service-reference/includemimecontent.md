---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: O elemento IncludeMimeContent especifica se o conteúdo MIME (Extensões de Email da Internet Multipropósitos) de um item ou anexo é retornado na resposta.
ms.openlocfilehash: 04d015ea450907f3968200dcbb6f411eb6343681
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542173"
---
# <a name="includemimecontent"></a>IncludeMimeContent

O **elemento IncludeMimeContent** especifica se o conteúdo MIME (Extensões de Email da Internet Multipropósitos) de um item ou anexo é retornado na resposta. 
  
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
|[AttachmentShape](attachmentshape.md) <br/> | Identifica propriedades adicionais a retornar em uma resposta a uma [solicitação GetAttachment.](getattachment.md)  <br/> <br/> Veja a seguir a expressão XPath para este elemento:  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/> <br/> Veja a seguir as expressões XPath para este elemento:<br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento pode ser **verdadeiro ou** **falso.** O valor padrão é **falso**. Esse é um tipo de dados Boolean.
  
## <a name="remarks"></a>Comentários

Esse elemento é opcional.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação demonstra como definir o **elemento IncludeMimeContent.** 
  
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

O atributo Id do anexo é truncado para preservar a capacidade de leitura.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

