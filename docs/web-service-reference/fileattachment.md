---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: O elemento FileAttachment representa um arquivo anexado a um item no Exchange store.
ms.openlocfilehash: 66424fefafd2084bf0b6f45881089448593e621d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518495"
---
# <a name="fileattachment"></a>FileAttachment

O **elemento FileAttachment** representa um arquivo anexado a um item no Exchange store. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifica o anexo de arquivo.  <br/> |
|[Name (AttachmentType)](name-attachmenttype.md) <br/> |Representa o nome do anexo.  <br/> |
|[ContentType](contenttype.md) <br/> |Descreve o tipo MIME (Extensões de Email da Internet) multiuso do conteúdo de anexo.  <br/> |
|[ContentId](contentid.md) <br/> |Representa um identificador para o conteúdo de um anexo. [ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres. Os aplicativos podem [usar ContentId](contentid.md) para implementar seus próprios mecanismos de identificação.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contém o URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho em bytes do anexo de arquivo.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Representa quando o anexo de arquivo foi modificado pela última vez.  <br/> |
|[IsInline](isinline.md) <br/> |Representa se o anexo aparece em linha dentro de um item.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Indica se o anexo de arquivo é uma imagem de contato.  <br/> |
|[Conteúdo](content.md) <br/> |Contém o conteúdo codificado em Base64 do anexo de arquivo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

