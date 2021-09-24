---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: O elemento GetServiceConfiguration define uma solicitação GetServiceConfiguration.
ms.openlocfilehash: fdc4fd84c658dd0cd2ecabe7fefc06113bca173a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533431"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

O **elemento GetServiceConfiguration** define uma solicitação GetServiceConfiguration. 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 **GetServiceConfigurationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifica quem o chamador está enviando como. Esse elemento é opcional. Se esse elemento não estiver presente, o usuário autenticado será assumido como o remetente. O **elemento ActingAs** deve ser incluído para solicitar dicas de remetente. Um erro ErrorInvalidArgument pode ser retornado em uma resposta se o elemento **ActingAs** estiver ausente, não incluir um tipo de roteamento, não incluir um endereço de email, contém um endereço de email inválido, não resolve para um usuário no Active Directory Domain Services (AD DS) ou resolve para vários usuários no AD DS.  <br/> |
|[RequestedConfiguration](requestedconfiguration.md) <br/> |Contém as configurações de serviço solicitadas. Este elemento é obrigatório.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

