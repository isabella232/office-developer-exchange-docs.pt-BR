---
title: ActingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: O elemento ActingAs identifica quem o chamador está enviando como.
ms.openlocfilehash: a470a7571e5f1b2ecc85014157d3fc4de291389e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540333"
---
# <a name="actingas"></a>ActingAs

O **elemento ActingAs** identifica quem o chamador está enviando como. 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetServiceConfiguration](getserviceconfiguration.md) <br/> |Define uma **solicitação GetServiceConfiguration.**  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é opcional. Se esse elemento não estiver presente, o usuário autenticado será assumido como o remetente. O **elemento ActingAs** deve ser incluído para solicitar dicas de remetente. Um **erro ErrorInvalidArgument** pode ser retornado em uma resposta se o elemento **ActingAs** estiver ausente, não incluir um tipo de roteamento, não incluir um endereço de email, contém um endereço de email inválido, não resolve para um usuário no Active Directory Domain Services (AD DS) ou resolve para vários usuários no AD DS. 
  
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

