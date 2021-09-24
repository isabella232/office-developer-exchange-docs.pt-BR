---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: O elemento PrimarySmtpAddress representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para autorização de servidor para servidor ou acesso delegado.
ms.openlocfilehash: 7963fbc92de88b38da93e577ebd2c39dbedac009
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523871"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

O **elemento PrimarySmtpAddress** representa o endereço SMTP (Simple Mail Transfer Protocol) principal de uma conta a ser usada para autorização de servidor para servidor ou acesso delegado. 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Representa uma conta para representar quando você está usando o header SOAP do ExchangeImpersonation.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Usado no header SOAP para serialização de token na autenticação servidor para servidor.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso à pasta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um endereço SMTP é necessário.
  
## <a name="remarks"></a>Comentários

Exchange Os Serviços Web exigem que as caixas de correio sejam identificadas pelo endereço SMTP principal da caixa de correio. Proxy ou endereços alternativos não são aceitos.
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Autorização de servidor para servidor no EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[Trabalhando com o Delegate Access](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

