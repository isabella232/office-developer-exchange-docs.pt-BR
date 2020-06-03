---
title: Identificar a conta a ser representada
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Saiba como o aplicativo de serviço usa EWS para identificar o usuário a ser personificado.
localization_priority: Priority
ms.openlocfilehash: 7159707abe96632aba2ed70dc0057417e087349f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527989"
---
# <a name="identify-the-account-to-impersonate"></a>Identificar a conta a ser representada

Saiba como o aplicativo de serviço usa EWS para identificar o usuário a ser personificado.
  
O aplicativo de serviço identifica a conta de usuário para representar usando um dos três identificadores a seguir:
  
- O endereço SMTP principal.
    
- O nome principal do usuário (UPN).
    
- O identificador de segurança (SID).
    
O identificador que você usa depende, naturalmente, nas informações disponíveis no seu aplicativo.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Identificando a conta de usuário para representar

Seu aplicativo pode usar as solicitações de API gerenciada do EWS ou do EWS SOAP para identificar a conta de usuário que está representando. A API gerenciada do EWS usa a propriedade [ExchangeService. ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para identificar o usuário representado. O EWS usa o elemento [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , conforme mostrado no fragmento XML a seguir. 
  
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
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Usar o endereço de email SMTP para identificar a conta de usuário

O endereço de email SMTP é o endereço de email principal associado a uma conta de usuário.
  
Em um aplicativo da API gerenciada por EWS, você especifica o endereço de email SMTP junto com o valor de enumeração [ConnectingIdType. SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

Em uma solicitação SOAP do EWS, o elemento [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contém o endereço de email da conta de usuário. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>Usar o UPN para identificar a conta de usuário

O UPN contém o nome de domínio totalmente qualificado (FQDN) para o local da conta de usuário. Isso não é necessariamente o domínio de caixa de correio do usuário. O atributo **userPrincipalName** deve ser definido corretamente na conta de usuário no AD DS (serviços de domínio Active Directory) para que a pesquisa do usuário seja bem-sucedida. 
  
Em um aplicativo da API gerenciada por EWS, você especifica o UPN junto com o valor de enumeração [ConnectingIdType. PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

Em uma solicitação SOAP do EWS, o elemento [ElementName (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) contém o UPN da conta de usuário. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>Usar o SID para identificar a conta de usuário

O SID é o identificador da conta a ser representada em Security Descriptor Definition Language (SDDL) Form.
  
Em um aplicativo da API gerenciada por EWS, você especifica o SID junto com o valor de enumeração [ConnectingIdType. Sid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

Em uma solicitação SOAP do EWS, o elemento [Sid](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contém o SID da conta de usuário. 
  
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
    
- [Classe ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

