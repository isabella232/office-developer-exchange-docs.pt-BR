---
title: Identificar a conta para representar
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Saiba como o aplicativo de serviço usa o EWS para identificar o usuário para representar.
ms.openlocfilehash: 78df4b511a9947d4d815b2802a53ab178b14622b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750725"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="f8397-103">Identificar a conta para representar</span><span class="sxs-lookup"><span data-stu-id="f8397-103">Identify the account to impersonate</span></span>

<span data-ttu-id="f8397-104">Saiba como o aplicativo de serviço usa o EWS para identificar o usuário para representar.</span><span class="sxs-lookup"><span data-stu-id="f8397-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="f8397-105">Seu aplicativo de serviço identifica a conta de usuário para representar usando um dos três identificadores a seguir:</span><span class="sxs-lookup"><span data-stu-id="f8397-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="f8397-106">O endereço SMTP principal.</span><span class="sxs-lookup"><span data-stu-id="f8397-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="f8397-107">O nome de princípio de usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="f8397-107">The user principle name (UPN).</span></span>
    
- <span data-ttu-id="f8397-108">O identificador de segurança (SID).</span><span class="sxs-lookup"><span data-stu-id="f8397-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="f8397-109">O identificador que você usa depende, obviamente, as informações que seu aplicativo tenha disponíveis.</span><span class="sxs-lookup"><span data-stu-id="f8397-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="f8397-110">Identifica a conta de usuário para representar</span><span class="sxs-lookup"><span data-stu-id="f8397-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="f8397-111">Seu aplicativo pode usar a API gerenciada de EWS ou o EWS SOAP solicitações para identificar a conta de usuário que está representando.</span><span class="sxs-lookup"><span data-stu-id="f8397-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="f8397-112">A API gerenciada de EWS usa a propriedade [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) para identificar o usuário representado.</span><span class="sxs-lookup"><span data-stu-id="f8397-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="f8397-113">EWS usa o elemento [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , conforme mostrado no fragmento XML a seguir.</span><span class="sxs-lookup"><span data-stu-id="f8397-113">EWS uses the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="f8397-114">Cada uma das seções a seguir mostra como usar um dos identificadores.</span><span class="sxs-lookup"><span data-stu-id="f8397-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="f8397-115">Para obter um exemplo que mostra o identificador de representação em ação, consulte [Adicionar compromissos usando a representação do Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="f8397-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="f8397-116">Use o endereço de email SMTP para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="f8397-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="f8397-117">O endereço de email SMTP é o endereço de email primário que está associado uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8397-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="f8397-118">Em um aplicativo do EWS Managed API, você deve especificar o endereço de email SMTP juntamente com o valor de enumeração [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f8397-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="f8397-119">Em uma solicitação SOAP EWS, o elemento [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contém o endereço de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8397-119">In an EWS SOAP request, the [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="f8397-120">Use o UPN para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="f8397-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="f8397-121">O UPN contém o nome de domínio totalmente qualificado (FQDN) para o local da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8397-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="f8397-122">Isso não é necessariamente o domínio do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f8397-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="f8397-123">O atributo **UserPrincipleName** deve ser definido corretamente na conta de usuário nos serviços de domínio Active Directory (AD DS) para a pesquisa de usuário ter sucesso.</span><span class="sxs-lookup"><span data-stu-id="f8397-123">The **UserPrincipleName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="f8397-124">Em um aplicativo do EWS Managed API, você deve especificar o UPN juntamente com o valor de enumeração [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f8397-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

<span data-ttu-id="f8397-125">Em uma solicitação SOAP EWS, o [PrincipalName elemento (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) elemento contém o UPN para a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8397-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="f8397-126">Use o SID para identificar a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="f8397-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="f8397-127">O SID é o identificador da conta a ser representada no formulário de idioma (SDDL) de definição de descritor de segurança.</span><span class="sxs-lookup"><span data-stu-id="f8397-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="f8397-128">Em um aplicativo do EWS Managed API, você deve especificar o SID juntamente com o valor de enumeração [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f8397-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="f8397-129">Em uma solicitação SOAP EWS, o elemento de [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contém o SID para a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8397-129">In an EWS SOAP request, the [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="f8397-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="f8397-130">See also</span></span>


- [<span data-ttu-id="f8397-131">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8397-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f8397-132">Adicione os compromissos, usando a representação do Exchange</span><span class="sxs-lookup"><span data-stu-id="f8397-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="f8397-133">Classe ExchangeService</span><span class="sxs-lookup"><span data-stu-id="f8397-133">ExchangeService class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="f8397-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f8397-134">ExchangeImpersonation</span></span>](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

