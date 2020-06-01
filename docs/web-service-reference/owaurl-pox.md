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
description: O elemento OWAUrl descreve a URL e o esquema de autenticação usados para acessar um determinado computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que hospeda o Outlook Web Access.
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457260"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

O elemento **OWAUrl** descreve a URL e o esquema de autenticação usados para acessar um determinado computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que hospeda o Outlook Web Access. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Interno (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Descreve os métodos de autenticação para acessar o Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Atributo AuthenticationMethod

|**Valor**|**Descrição**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Autenticação integrada do Windows.  <br/> |
|FBA  <br/> |Autenticação baseada em formulários.  <br/> |
|NTLM  <br/> |Autenticação NTLM.  <br/> |
|Digest  <br/> |Autenticação Digest.  <br/> |
|Básica  <br/> |Autenticação básica.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Interno (POX)](internal-pox.md) <br/> |Contém a coleção de URLs do Outlook Web Access às quais um cliente pode se conectar quando está dentro do firewall.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a URL do serviço do Outlook Web Access em um servidor de acesso para cliente.
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

