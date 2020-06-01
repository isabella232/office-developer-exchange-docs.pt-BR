---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: O elemento GetServiceConfiguration define uma solicitação GetServiceConfiguration.
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457869"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

O elemento **GetServiceConfiguration** define uma solicitação GetServiceConfiguration. 
  
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
|[Agindo](actingas.md) <br/> |Identifica quem o chamador está enviando como. Este elemento é opcional. Se esse elemento não estiver presente, o usuário autenticado será considerado como o remetente. O elemento **agindo** deve ser incluído para solicitar dicas de remetente. Um erro ErrorInvalidArgument pode ser retornado em uma resposta se o elemento **agindo** estiver ausente, não incluir um tipo de roteamento, não incluir um endereço de email, contiver um endereço de email inválido, não resolver para um usuário nos serviços de domínio do Active Directory (AD DS) ou resolver para vários usuários no AD DS.  <br/> |
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

