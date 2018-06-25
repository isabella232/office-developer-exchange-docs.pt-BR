---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: O elemento de GetSharingMetadata define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é a base para a operação GetSharingMetadata.
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823677"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

O elemento de **GetSharingMetadata** define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é a base para a [operação GetSharingMetadata](getsharingmetadata-operation.md).
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |Representa o identificador da pasta no servidor que será compartilhado. Este elemento é obrigatório.  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Representa o endereço de email SMTP que corresponde à caixa de correio que contém a pasta que é identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) . Este elemento é obrigatório.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Representa os endereços de email SMTP de uma ou mais entidades que receberão acesso aos dados na pasta que é identificado pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) . Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

