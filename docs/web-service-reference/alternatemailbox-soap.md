---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: O elemento AlternateMailbox representa uma caixa de correio alternativa.
ms.openlocfilehash: 3646efef9b63b2af8dbba41a07a86462e18ac1c1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543720"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

O **elemento AlternateMailbox** representa uma caixa de correio alternativa. 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 **AlternateMailbox**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Type (SOAP)](type-soap.md) <br/> |Representa o tipo de caixa de correio alternativo.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Representa o nome de exibição de caixa de correio alternativo.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Representa o nome diferenciado da caixa de correio alternativa herdados.  <br/> |
|[Server (SOAP)](server-soap.md) <br/> |Representa o servidor de caixa de correio alternativo.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Representa o endereço SMTP de caixa de correio alternativo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Representa uma coleção de caixas de correio alternativas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

