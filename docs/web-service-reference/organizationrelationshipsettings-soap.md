---
title: OrganizationRelationshipSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: O elemento OrganizationRelationshipSettings representa uma lista de relações de organização para uma única organização. O elemento OrganizationRelationshipSettings é apenas para uso interno. Esse elemento não é usado pelos clientes.
ms.openlocfilehash: bff515456d6f86648417070008845b7b5caa6d8a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514246"
---
# <a name="organizationrelationshipsettings-soap"></a>OrganizationRelationshipSettings (SOAP)

O **elemento OrganizationRelationshipSettings** representa uma lista de relações de organização para uma única organização. O **elemento OrganizationRelationshipSettings** é apenas para uso interno. Esse elemento não é usado pelos clientes. 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 **OrganizationRelationshipSettings**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeliveryReportEnabled (SOAP)](deliveryreportenabled-soap.md) <br/> |Representa o [sinalizador DeliveryReportEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx)  <br/> |
|[DomainNames (SOAP)](domainnames-soap.md) <br/> |Representa a coleção de nomes de domínio.  <br/> |
|[FreeBusyAccessEnabled (SOAP)](freebusyaccessenabled-soap.md) <br/> |Representa o [sinalizador FreeBusyAccessEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx)  <br/> |
|[FreeBusyAccessLevel (SOAP)](freebusyaccesslevel-soap.md) <br/> |Representa a [propriedade FreeBusyAccessLevel.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx)  <br/> |
|[MailTipsAccessEnabled (SOAP)](mailtipsaccessenabled-soap.md) <br/> |Representa o [sinalizador MailTipsAccessEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx)  <br/> |
|[MailTipsAccessLevel (SOAP)](mailtipsaccesslevel-soap.md) <br/> |Representa a [propriedade MailTipsAccessLevel.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx)  <br/> |
|[MailboxMoveEnabled (SOAP)](mailboxmoveenabled-soap.md) <br/> |Representa o [sinalizador MailboxMoveEnabled().](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx)  <br/> |
|[Name (SOAP)](name-soap.md) <br/> |Representa o nome da relação da organização.  <br/> |
|[TargetApplicationUri (SOAP)](targetapplicationuri-soap.md) <br/> |Define o URI do aplicativo de destino.  <br/> |
|[TargetAutodiscoverEpr (SOAP)](targetautodiscoverepr-soap.md) <br/> |Representa a [propriedade TargetAutodiscoverEpr.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx)  <br/> |
|[TargetSharingEpr (SOAP)](targetsharingepr-soap.md) <br/> |Representa a [propriedade TargetSharingEpr.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Representa uma lista de relações de organização que corresponde à consulta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   

