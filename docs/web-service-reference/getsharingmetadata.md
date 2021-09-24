---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: O elemento GetSharingMetadata define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Esse elemento é o elemento base da operação GetSharingMetadata.
ms.openlocfilehash: 65da8371b25c42e59f898c79403f06fa17e5a24a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523045"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

O **elemento GetSharingMetadata** define uma solicitação para obter um token de autenticação opaco que identifica o convite de compartilhamento. Esse elemento é o elemento base da [operação GetSharingMetadata](getsharingmetadata-operation.md).
  
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
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Representa o endereço de email SMTP que corresponde à caixa de correio que contém a pasta identificada pelo [elemento IdOfFolderToShare.](idoffoldertoshare.md) Este elemento é obrigatório.  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Representa os endereços de email SMTP de uma ou mais entidades que terão acesso aos dados na pasta identificada pelo elemento [IdOfFolderToShare.](idoffoldertoshare.md) Este elemento é obrigatório.  <br/> |
   
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

