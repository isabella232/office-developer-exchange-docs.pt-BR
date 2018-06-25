---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: O elemento FileAttachment representa um arquivo anexado a um item no armazenamento do Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752252"
---
# <a name="fileattachment"></a>FileAttachment

O elemento **FileAttachment** representa um arquivo anexado a um item no armazenamento do Exchange. 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 **FileAttachmentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifica o anexo de arquivo.  <br/> |
|[Nome (AttachmentType)](name-attachmenttype.md) <br/> |Representa o nome do anexo.  <br/> |
|[ContentType](contenttype.md) <br/> |Descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.  <br/> |
|[ContentId](contentid.md) <br/> |Representa um identificador para o conteúdo de um anexo. [ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres. Aplicativos podem usar [ContentId](contentid.md) implementar seus próprios mecanismos de identificação.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo do anexo.  <br/> |
|[Size](size.md) <br/> |Representa o tamanho em bytes de arquivo do anexo.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Representa quando o anexo de arquivo foi modificado pela última vez.  <br/> |
|[IsInline](isinline.md) <br/> |Indica se o anexo é exibido embutida dentro de um item.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Indica se o anexo de arquivo é uma imagem do contato.  <br/> |
|[Conteúdo](content.md) <br/> |Contém o conteúdo codificado na Base64 de arquivo do anexo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

