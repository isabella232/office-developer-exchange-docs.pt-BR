---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: O elemento OWAUrl descreve a URL e o esquema de autenticação que é usado para acessar um computador específico que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada que hospeda o Outlook Web Access.
ms.openlocfilehash: fbd61eb75018c57dada40f5ed7472379d365e752
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534888"
---
# <a name="owaurl-pox"></a>OWAUrl (POX)

O **elemento OWAUrl** descreve a URL e o esquema de autenticação que é usado para acessar um determinado computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada que hospeda o Outlook Web Access. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Internal (POX)](internal-pox.md)
  
[OWAUrl (POX)](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**AuthenticationMethod** <br/> |Descreve os métodos de autenticação para acessar Outlook Web Access.  <br/> |
   
#### <a name="authenticationmethod-attribute"></a>Atributo AuthenticationMethod

|**Valor**|**Descrição**|
|:-----|:-----|
|WindowsIntegrated  <br/> |Autenticação Windows integrada.  <br/> |
|FBA  <br/> |Autenticação baseada em formulários.  <br/> |
|NTLM  <br/> |Autenticação NTLM.  <br/> |
|Compilação  <br/> |Autenticação digest.  <br/> |
|Básico  <br/> |Autenticação básica.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Internal (POX)](internal-pox.md) <br/> |Contém a coleção de Outlook URLs do Web Access às que um cliente pode se conectar quando está dentro do firewall.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a URL do serviço Outlook Web Access em um servidor de Acesso para Cliente.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

