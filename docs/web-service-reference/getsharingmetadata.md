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
description: O elemento GetSharingMetadata define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é o elemento base para a operação GetSharingMetadata.
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530843"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

O elemento **GetSharingMetadata** define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Este elemento é o elemento base para a [operação GetSharingMetadata](getsharingmetadata-operation.md).
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |Representa o identificador da pasta no servidor que será compartilhado. Este elemento é obrigatório.  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Representa o endereço de email SMTP que corresponde à caixa de correio que contém a pasta identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) . Este elemento é obrigatório.  <br/> |
|[Destinatários (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Representa os endereços de email SMTP de uma ou mais entidades que terão acesso aos dados na pasta identificada pelo elemento [IdOfFolderToShare](idoffoldertoshare.md) . Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

