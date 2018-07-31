---
title: Identificar a conta para representar
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Saiba como o aplicativo de serviço usa o EWS para identificar o usuário para representar.
ms.openlocfilehash: 01c6ee797359c38c8539257003a2f110fdf253cf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354292"
---
# <a name="identify-the-account-to-impersonate"></a>Identificar a conta para representar

Saiba como o aplicativo de serviço usa o EWS para identificar o usuário para representar.
  
Seu aplicativo de serviço identifica a conta de usuário para representar usando um dos três identificadores a seguir:
  
- O endereço SMTP principal.
    
- O nome de princípio de usuário (UPN).
    
- O identificador de segurança (SID).
    
O identificador que você usa depende, obviamente, as informações que seu aplicativo tenha disponíveis.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Identifica a conta de usuário para representar

Seu aplicativo pode usar a API gerenciada de EWS ou o EWS SOAP solicitações para identificar a conta de usuário que está representando. A API gerenciada de EWS usa a propriedade [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para identificar o usuário representado. EWS usa o elemento [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , conforme mostrado no fragmento XML a seguir. 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

Cada uma das seções a seguir mostra como usar um dos identificadores. Para obter um exemplo que mostra o identificador de representação em ação, consulte [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Use o endereço de email SMTP para identificar a conta de usuário

O endereço de email SMTP é o endereço de email primário que está associado uma conta de usuário.
  
Em um aplicativo do EWS Managed API, você deve especificar o endereço de email SMTP juntamente com o valor de enumeração [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

Em uma solicitação SOAP EWS, o elemento [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contém o endereço de email da conta de usuário. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>Use o UPN para identificar a conta de usuário

O UPN contém o nome de domínio totalmente qualificado (FQDN) para o local da conta de usuário. Isso não é necessariamente o domínio do usuário da caixa de correio. O atributo **UserPrincipleName** deve ser definido corretamente na conta de usuário nos serviços de domínio Active Directory (AD DS) para a pesquisa de usuário ter sucesso. 
  
Em um aplicativo do EWS Managed API, você deve especificar o UPN juntamente com o valor de enumeração [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

Em uma solicitação SOAP EWS, o [PrincipalName elemento (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) elemento contém o UPN para a conta de usuário. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>Use o SID para identificar a conta de usuário

O SID é o identificador da conta a ser representada no formulário de idioma (SDDL) de definição de descritor de segurança.
  
Em um aplicativo do EWS Managed API, você deve especificar o SID juntamente com o valor de enumeração [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

Em uma solicitação SOAP EWS, o elemento de [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contém o SID para a conta de usuário. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a>Confira também


- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
    
- [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [Classe ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

