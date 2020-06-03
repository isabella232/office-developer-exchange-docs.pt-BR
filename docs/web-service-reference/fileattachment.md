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
description: O elemento fileattachment representa um arquivo anexado a um item no repositório do Exchange.
ms.openlocfilehash: db9b541fb2527ae3c09cbdb33bedea7fb215bd30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461013"
---
# <a name="fileattachment"></a>FileAttachment

O elemento **Fileattachment** representa um arquivo anexado a um item no repositório do Exchange. 
  
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
|[Attachmentid](attachmentid.md) <br/> |Identifica o anexo de arquivo.  <br/> |
|[Nome (AttachmentType)](name-attachmenttype.md) <br/> |Representa o nome do anexo.  <br/> |
|[ContentType](contenttype.md) <br/> |Descreve o tipo de MIME (Multipurpose Internet Mail Extensions) do conteúdo do anexo.  <br/> |
|[ContentId](contentid.md) <br/> |Representa um identificador para o conteúdo de um anexo. [ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres. Os aplicativos podem usar [ContentId](contentid.md) para implementar seus próprios mecanismos de identificação.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contém o URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho em bytes do anexo de arquivo.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Representa quando o anexo de arquivo foi modificado pela última vez.  <br/> |
|[IsInline](isinline.md) <br/> |Indica se o anexo aparece embutido em um item.  <br/> |
|[IsContactPhoto](iscontactphoto.md) <br/> |Indica se o anexo de arquivo é uma imagem de contato.  <br/> |
|[Conteúdo](content.md) <br/> |Contém o conteúdo codificado em base64 do anexo de arquivo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

