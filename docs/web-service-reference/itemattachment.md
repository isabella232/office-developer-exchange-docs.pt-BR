---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: O elemento ItemAttachment representa um item do Exchange que está anexado a outro item do Exchange.
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824137"
---
# <a name="itemattachment"></a>ItemAttachment

O elemento **ItemAttachment** representa um item do Exchange que está anexado a outro item do Exchange. 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

 **ItemAttachmentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentId](attachmentid.md) <br/> |Identifica o anexo.  <br/> |
|[Nome (AttachmentType)](name-attachmenttype.md) <br/> |Representa o nome do anexo.  <br/> |
|[ContentType](contenttype.md) <br/> |Descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.  <br/> |
|[ContentId](contentid.md) <br/> |Representa um identificador para o conteúdo do anexo. [ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres. Aplicativos podem usar [ContentId](contentid.md) implementar seus próprios mecanismos de identificação.  <br/> |
|[ContentLocation](contentlocation.md) <br/> |Contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo do anexo.  <br/> |
|[Size](size.md) <br/> |Representa o tamanho em bytes de arquivo do anexo.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Representa quando o anexo foi modificado pela última vez.  <br/> |
|[IsInline](isinline.md) <br/> |Indica se o anexo é exibido embutida dentro de um item.  <br/> |
|[1.1](item.md) <br/> |Representa um anexo de item genérico do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa um anexo de mensagem de email do Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Representa um anexo de item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um anexo de item de contato do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa um anexo de tarefa do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os arquivos que estejam anexados a um item no armazenamento do Exchange e/ou itens.  <br/> |
   
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
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

