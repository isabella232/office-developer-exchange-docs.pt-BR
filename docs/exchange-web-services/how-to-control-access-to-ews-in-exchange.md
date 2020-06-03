---
title: Controlar o acesso ao EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Descubra como controlar o acesso ao EWS para usuários, aplicativos ou para toda a organização.
localization_priority: Priority
ms.openlocfilehash: bd65b099ab15c1514945d8a1cfa4e9b1428a4755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456875"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="d86f3-103">Controlar o acesso ao EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d86f3-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="d86f3-104">Descubra como controlar o acesso ao EWS para usuários, aplicativos ou para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="d86f3-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="d86f3-105">Se você estiver usando a API gerenciada do EWS ou o EWS diretamente, em seu aplicativo, você pode controlar o acesso aos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d86f3-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="d86f3-106">Se tiver acesso de administrador ao seu servidor Exchange, você poderá gerenciar o acesso ao EWS usando o Shell de gerenciamento do Exchange para controlar o acesso globalmente, para cada usuário e para cada aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d86f3-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="d86f3-107">Cmdlets do Shell de gerenciamento do Exchange para configurar o controle de acesso</span><span class="sxs-lookup"><span data-stu-id="d86f3-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="d86f3-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="d86f3-108"><a name="bk_Cmdlets"> </a></span></span>

<span data-ttu-id="d86f3-109">Você pode usar os seguintes cmdlets do Shell de gerenciamento do Exchange para exibir a configuração atual do Access e definir os controles de acesso do EWS:</span><span class="sxs-lookup"><span data-stu-id="d86f3-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="d86f3-110">[Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) -mostra quais parâmetros estão definidos para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="d86f3-110">[Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="d86f3-111">[Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) -define parâmetros para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="d86f3-111">[Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="d86f3-112">[Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) -mostra os parâmetros para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="d86f3-112">[Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="d86f3-113">[Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) -define os parâmetros de toda a organização.</span><span class="sxs-lookup"><span data-stu-id="d86f3-113">[Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="d86f3-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="d86f3-114"><a name="bk_Examples"> </a></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="d86f3-115">Exemplos: controle de acesso ao EWS</span><span class="sxs-lookup"><span data-stu-id="d86f3-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="d86f3-116">Vamos dar uma olhada em alguns cenários que mostram como você pode controlar o acesso ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d86f3-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="d86f3-117">**Tabela 1. Comandos para controlar o acesso ao EWS**</span><span class="sxs-lookup"><span data-stu-id="d86f3-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="d86f3-118">Se você desejar</span><span class="sxs-lookup"><span data-stu-id="d86f3-118">If you want to</span></span> |<span data-ttu-id="d86f3-119">Use este comando</span><span class="sxs-lookup"><span data-stu-id="d86f3-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="d86f3-120">Bloquear o uso de todos os aplicativos cliente do EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="d86f3-121">Isso permite que os aplicativos listados na lista de permissões para se conectar.</span><span class="sxs-lookup"><span data-stu-id="d86f3-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="d86f3-122">Neste exemplo, nenhum aplicativo está incluído no Allowlist, portanto, nenhum aplicativo pode usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="d86f3-123">Permite que uma lista de aplicativos cliente use EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="d86f3-124">Isso permite que aplicativos específicos usem EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="d86f3-125">Neste exemplo, qualquer aplicativo que tenha uma cadeia de caracteres de agente de usuário que comece com "OWA/" tem permissão de acesso.</span><span class="sxs-lookup"><span data-stu-id="d86f3-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="d86f3-126">Permitir que todos os aplicativos cliente usem EWS, exceto aqueles especificamente bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d86f3-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="d86f3-127">Este exemplo apenas impede que aplicativos usem EWS que têm uma cadeia de caracteres de agente de usuário que começa com "OWA/".</span><span class="sxs-lookup"><span data-stu-id="d86f3-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="d86f3-128">Permitir que todos os aplicativos cliente usem o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="d86f3-129">Como nenhuma blocklist é especificada, todos os aplicativos podem usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="d86f3-130">Bloquear a organização inteira usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="d86f3-131">Permita que toda a organização Use o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="d86f3-132">Bloquear uma caixa de correio individual usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="d86f3-133">Permitir que uma caixa de correio individual use EWS.</span><span class="sxs-lookup"><span data-stu-id="d86f3-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="d86f3-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="d86f3-134">See also</span></span>

- [<span data-ttu-id="d86f3-135">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="d86f3-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="d86f3-136">Controlando o acesso do aplicativo cliente ao EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d86f3-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="d86f3-137">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="d86f3-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="d86f3-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d86f3-138">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

