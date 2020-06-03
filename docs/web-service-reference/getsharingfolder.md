---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: O elemento GetSharingFolder define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada. É o elemento base para a operação GetSharingFolder.
ms.openlocfilehash: cb76c534d9b30d0a9d1b267396551eb2871e638a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460502"
---
# <a name="getsharingfolder"></a>GetSharingFolder

O elemento **GetSharingFolder** define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada. É o elemento base para a [operação GetSharingFolder](getsharingfolder-operation.md).
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Representa o endereço de email SMTP da outra parte na relação de compartilhamento. Este elemento é obrigatório.  <br/> |
|[DataType](datatype.md) <br/> |Descreve o tipo de dados que é compartilhado por uma pasta compartilhada. Este elemento é opcional.  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |Representa o identificador da pasta compartilhada cujo identificador de pasta local deve ser retornado. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

Um elemento GetSharingFolder deve conter um elemento [smtpAddress](smtpaddress.md) . Um elemento GetSharingFolder também deve conter um elemento [DataType](datatype.md) ou um elemento [SharedFolderId](sharedfolderid.md) , mas não pode conter ambos. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetSharingFolder](getsharingfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

