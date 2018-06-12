---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: O elemento OWAUrl descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server 2007 que possui a função acesso para cliente instalada que hospeda o Outlook Web Access.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824673"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

O elemento **OWAUrl** descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server 2007 que possui a função acesso para cliente instalada que hospeda o Outlook Web Access. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[Interno (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Descreve os métodos de autenticação para acessar o Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Atributo AuthenticationMethod

|**Valor**|**Descrição**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Autenticação integrada do Windows.  <br/> |
|FBA  <br/> |Autenticação baseada em formulários.  <br/> |
|NTLM  <br/> |Autenticação NTLM.  <br/> |
|Digest  <br/> |Autenticação Digest.  <br/> |
|Básico  <br/> |Autenticação básica.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Interno (POX)](internal-pox.md) <br/> |Contém a coleção de URLs do Outlook Web Access que um cliente pode se conectar ao quando ele estiver dentro do firewall.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a URL do serviço do Outlook Web Access em um servidor de acesso para cliente.
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

