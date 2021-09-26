---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: O elemento ResponseCode fornece informações sobre por que o destinatário é inválido.
ms.openlocfilehash: 33cd05aca672e250f288aec72d876734132d2e36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544805"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

O **elemento ResponseCode** fornece informações sobre por que o destinatário é inválido. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento ResponseCode.** 
  
|**Código**|**Descrição**|
|:-----|:-----|
|OtherError  <br/> |Indica que o erro não é especificado por outro código de resposta de erro.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Indica que uma relação de compartilhamento não está disponível com a organização especificada no endereço de email SMTP do destinatário.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Indica que houve um problema ao obter um token de segurança do servidor de tokens.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Indica que o administrador do sistema definiu uma política de sistema que bloqueia o compartilhamento com o destinatário especificado.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Indica que o serviço de token seguro usado pelo destinatário especificado é desconhecido.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetSharingMetadata](getsharingmetadata-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

