---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: O elemento AlternateMailbox representa uma caixa de correio alternativa.
ms.openlocfilehash: 9019f85a373cc186cc9dadddceee3dc9d11b3854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466154"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

O elemento **AlternateMailbox** representa uma caixa de correio alternativa. 
  
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
|[Tipo (SOAP)](type-soap.md) <br/> |Representa o tipo de caixa de correio alternativa.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Representa o nome de exibição alternativo da caixa de correio.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Representa o nome diferenciado herdado da caixa de correio.  <br/> |
|[Servidor (SOAP)](server-soap.md) <br/> |Representa o servidor de caixa de correio alternativo.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Representa o endereço SMTP alternativo da caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Representa uma coleção de caixas de correio alternadas.  <br/> |
   
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

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

