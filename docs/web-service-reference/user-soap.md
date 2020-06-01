---
title: Usuário (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: O elemento user representa a identidade de um único usuário.
ms.openlocfilehash: f151ffa8050a10cdbb4562471d815f8692596cc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456343"
---
# <a name="user-soap"></a>Usuário (SOAP)

O elemento **User** representa a identidade de um único usuário. 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 **Usuário**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Representa o nome diferenciado herdado da caixa de correio.  <br/> |
|[Caixa de correio (SOAP)](mailbox-soap.md) <br/> |Contém o endereço de email do usuário a ser descoberto.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das definições de configuração solicitadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuários (SOAP)](users-soap.md) <br/> |Representa uma coleção de elementos do **usuário** .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Operação GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

