---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: O elemento ResponseCode fornece informações sobre por que o destinatário é inválido.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

O elemento **ResponseCode** fornece informações sobre por que o destinatário é inválido. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **ResponseCode** . 
  
|**Code**|**Descrição**|
|:-----|:-----|
|OtherError  <br/> |Indica que o erro não for especificado por outro código de resposta de erro.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Indica que uma relação de compartilhamento não está disponível com a organização especificada no endereço de email SMTP do destinatário.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Indica que houve um problema ao obter um token de segurança do servidor de token.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Indica que o administrador do sistema tiver definido uma diretiva de sistema que bloqueia o compartilhamento com o destinatário especificado.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Indica que o serviço de token seguro que é usado pelo destinatário especificado é desconhecido.  <br/> |
   
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



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

