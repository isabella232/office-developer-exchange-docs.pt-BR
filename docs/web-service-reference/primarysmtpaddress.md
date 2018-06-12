---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: O elemento PrimarySmtpAddress representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para autorização de servidor-para-servidor ou acesso de representante.
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824881"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

O elemento **PrimarySmtpAddress** representa o endereço de Simple Mail Transfer Protocol (SMTP) principal de uma conta a ser usada para autorização de servidor-para-servidor ou acesso de representante. 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar quando você estiver usando o cabeçalho SOAP ExchangeImpersonation.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Usado no cabeçalho SOAP para serialização de token de autenticação de servidor-para-servidor.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um endereço SMTP.
  
## <a name="remarks"></a>Coment�rios

Serviços Web do Exchange requer que as caixas de correio ser identificado pelo endereço SMTP principal da caixa de correio. Proxy ou endereços alternativos não são aceitas.
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Autorização de servidor-para-servidor no EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[Trabalhando com acesso de representante](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

