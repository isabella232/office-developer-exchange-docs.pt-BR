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
description: O elemento de GetSharingFolder define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada. É o elemento de base para a operação GetSharingFolder.
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823669"
---
# <a name="getsharingfolder"></a>GetSharingFolder

O elemento de **GetSharingFolder** define uma solicitação para obter o identificador de pasta local de uma pasta compartilhada especificada. É o elemento de base para a [operação GetSharingFolder](getsharingfolder-operation.md).
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Representa o endereço de email SMTP da outra na relação de compartilhamento. Este elemento é obrigatório.  <br/> |
|[Tipo de dados](datatype.md) <br/> |Descreve o tipo de dados que são compartilhados por uma pasta compartilhada. Esse elemento é opcional.  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |Representa o identificador da pasta compartilhada cujo identificador de pasta local deve ser retornado. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Um elemento GetSharingFolder deve conter um elemento [SmtpAddress](smtpaddress.md) . Um elemento GetSharingFolder também deve conter um elemento [DataType](datatype.md) ou um elemento [SharedFolderId](sharedfolderid.md) , mas não pode conter ambos. 
  
O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetSharingFolder](getsharingfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

