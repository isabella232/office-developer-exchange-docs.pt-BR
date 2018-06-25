---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: O elemento BodyType identifica como o corpo de texto é formatado na resposta.
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751305"
---
# <a name="bodytype"></a>BodyType

O elemento **BodyType** identifica como o corpo de texto é formatado na resposta. 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/><br/>A seguir estão as expressões XPath para esse elemento:<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifica as propriedades de item estendido adicional para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) .  <br/><br/>Este é a expressão XPath para esse elemento:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **BodyType** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Melhor  <br/> |A resposta retornará o conteúdo disponível mais sofisticado de corpo de texto. Isso é útil se for desconhecido se o conteúdo é o texto ou HTML.<br/><br/> O corpo retornado será o texto se o corpo armazenado for texto sem formatação. Caso contrário, a resposta retornará HTML, se o corpo armazenado está no formato HTML ou RTF.<br/><br/> Este é o valor padrão.  <br/> |
|HTML  <br/> |A resposta retornará o corpo de um item como HTML.  <br/> |
|Texto  <br/> |A resposta retornará o corpo de um item como texto sem formatação.  <br/> |
   
## <a name="remarks"></a>Comentários

Você pode identificar o tipo de corpo retornado na resposta, verificando o atributo **BodyType** do elemento [Body](body.md) . O atributo **BodyType** identificará o corpo como HTML ou texto. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação mostra onde um elemento **BodyType** é usado. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

O atributo Id foi reduzido para preservar a legibilidade.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

