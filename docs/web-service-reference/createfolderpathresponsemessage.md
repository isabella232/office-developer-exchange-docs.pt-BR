---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: O elemento CreateFolderPathResponseMessage especifica a mensagem de resposta de uma solicitação CreateFolderPath.
ms.openlocfilehash: ca2640ca18421260c0398c276c81f023664216ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526519"
---
# <a name="createfolderpathresponsemessage"></a>CreateFolderPathResponseMessage

O **elemento CreateFolderPathResponseMessage** especifica a mensagem de resposta de uma **solicitação CreateFolderPath.** 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 **FolderInfoResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|ResponseClass  <br/> |Indica a classe da resposta.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|Sucesso  <br/> |Indica sucesso.  <br/> |
|Aviso  <br/> |Indica um aviso.  <br/> |
|Erro  <br/> |Indica um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas que são usadas em operações de pasta.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro.  <br/> |
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece informações de status sobre a solicitação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação Exchange Web Services.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

