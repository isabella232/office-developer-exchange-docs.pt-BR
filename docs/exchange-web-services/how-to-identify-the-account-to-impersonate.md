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
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="ad3ba-103">Identificar a conta a ser representada</span><span class="sxs-lookup"><span data-stu-id="ad3ba-103">Identify the account to impersonate</span></span>

<span data-ttu-id="ad3ba-104">Saiba como o aplicativo de serviço usa EWS para identificar o usuário a ser personificado.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="ad3ba-105">O aplicativo de serviço identifica a conta de usuário para representar usando um dos três identificadores a seguir:</span><span class="sxs-lookup"><span data-stu-id="ad3ba-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="ad3ba-106">O endereço SMTP principal.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="ad3ba-107">O nome principal do usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="ad3ba-107">The user principal name (UPN).</span></span>
    
- <span data-ttu-id="ad3ba-108">O identificador de segurança (SID).</span><span class="sxs-lookup"><span data-stu-id="ad3ba-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="ad3ba-109">O identificador que você usa depende, naturalmente, nas informações disponíveis no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="ad3ba-110">Identificando a conta de usuário para representar</span><span class="sxs-lookup"><span data-stu-id="ad3ba-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="ad3ba-111">Seu aplicativo pode usar as solicitações de API gerenciada do EWS ou do EWS SOAP para identificar a conta de usuário que está representando.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="ad3ba-112">A API gerenciada do EWS usa a propriedade [ExchangeService. ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para identificar o usuário representado.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="ad3ba-113">O EWS usa o elemento [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , conforme mostrado no fragmento XML a seguir.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-113">EWS uses the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="ad3ba-114">Cada uma das seções a seguir mostra como usar um dos identificadores.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="ad3ba-115">Para obter um exemplo que mostra o identificador de representação em ação, consulte [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="ad3ba-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="ad3ba-116">Usar o endereço de email SMTP para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="ad3ba-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="ad3ba-117">O endereço de email SMTP é o endereço de email principal associado a uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="ad3ba-118">Em um aplicativo da API gerenciada por EWS, você especifica o endereço de email SMTP junto com o valor de enumeração [ConnectingIdType. SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ad3ba-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="ad3ba-119">Em uma solicitação SOAP do EWS, o elemento [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contém o endereço de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-119">In an EWS SOAP request, the [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="ad3ba-120">Usar o UPN para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="ad3ba-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="ad3ba-121">O UPN contém o nome de domínio totalmente qualificado (FQDN) para o local da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="ad3ba-122">Isso não é necessariamente o domínio de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="ad3ba-123">O atributo **userPrincipalName** deve ser definido corretamente na conta de usuário no AD DS (serviços de domínio Active Directory) para que a pesquisa do usuário seja bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-123">The **UserPrincipalName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="ad3ba-124">Em um aplicativo da API gerenciada por EWS, você especifica o UPN junto com o valor de enumeração [ConnectingIdType. PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ad3ba-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

<span data-ttu-id="ad3ba-125">Em uma solicitação SOAP do EWS, o elemento [ElementName (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) contém o UPN da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="ad3ba-126">Usar o SID para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="ad3ba-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="ad3ba-127">O SID é o identificador da conta a ser representada em Security Descriptor Definition Language (SDDL) Form.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="ad3ba-128">Em um aplicativo da API gerenciada por EWS, você especifica o SID junto com o valor de enumeração [ConnectingIdType. Sid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ad3ba-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="ad3ba-129">Em uma solicitação SOAP do EWS, o elemento [Sid](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contém o SID da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="ad3ba-129">In an EWS SOAP request, the [SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="ad3ba-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ad3ba-130">See also</span></span>


- [<span data-ttu-id="ad3ba-131">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ad3ba-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="ad3ba-132">Adicionar compromissos usando a representação do Exchange</span><span class="sxs-lookup"><span data-stu-id="ad3ba-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="ad3ba-133">Classe ExchangeService</span><span class="sxs-lookup"><span data-stu-id="ad3ba-133">ExchangeService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="ad3ba-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ad3ba-134">ExchangeImpersonation</span></span>](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

