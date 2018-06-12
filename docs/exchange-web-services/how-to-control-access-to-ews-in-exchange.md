---
title: Controlar o acesso a EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Descubra como controlar o acesso aos EWS para toda a organização, aplicativos ou usuários.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750696"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="43142-103">Controlar o acesso a EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43142-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="43142-104">Descubra como controlar o acesso aos EWS para toda a organização, aplicativos ou usuários.</span><span class="sxs-lookup"><span data-stu-id="43142-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="43142-105">Se você estiver usando a API gerenciada de EWS ou EWS diretamente, em seu aplicativo, você pode controlar o acesso a serviços de Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="43142-105">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS).</span></span> <span data-ttu-id="43142-106">Se você tiver acesso de administrador para o Exchange server, você pode gerenciar o acesso ao EWS usando o Shell de gerenciamento do Exchange para controlar o acesso globalmente, para cada usuário e para cada aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43142-106">If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="43142-107">Cmdlets do Shell de gerenciamento do Exchange para configurar o controle de acesso</span><span class="sxs-lookup"><span data-stu-id="43142-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="43142-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="43142-108"></span></span>

<span data-ttu-id="43142-109">Você pode usar os seguintes cmdlets do Shell de gerenciamento do Exchange para exibir a configuração atual do access e definir os controles de acesso do EWS:</span><span class="sxs-lookup"><span data-stu-id="43142-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="43142-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - mostra quais parâmetros são definidos para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="43142-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="43142-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - parâmetros de conjuntos para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="43142-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="43142-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - mostra os parâmetros para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="43142-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="43142-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - define os parâmetros para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="43142-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="43142-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="43142-114"></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="43142-115">Exemplos: Controlar o acesso às EWS</span><span class="sxs-lookup"><span data-stu-id="43142-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="43142-116">Vamos dar uma olhada em alguns cenários que mostram como você pode controlar o acesso ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43142-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="43142-117">**Tabela 1. Comandos para controlar o acesso às EWS**</span><span class="sxs-lookup"><span data-stu-id="43142-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="43142-118">Se você quiser</span><span class="sxs-lookup"><span data-stu-id="43142-118">If you want to</span></span> |<span data-ttu-id="43142-119">Use este comando</span><span class="sxs-lookup"><span data-stu-id="43142-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="43142-120">Impedir que todos os aplicativos cliente usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="43142-121">Isso permite que os aplicativos listados no AllowList para se conectar.</span><span class="sxs-lookup"><span data-stu-id="43142-121">This allows applications listed in the AllowList to connect.</span></span> <span data-ttu-id="43142-122">Neste exemplo, nenhum aplicativo é incluído no AllowList, para que nenhum aplicativo possa usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-122">In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="43142-123">Uma lista de cliente permitem que aplicativos usam o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="43142-124">Isso permite que aplicativos específicos para usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="43142-125">Neste exemplo, qualquer aplicativo que tenha um agente de usuário a cadeia de caracteres que começa com "OWA /" tem acesso permitido.</span><span class="sxs-lookup"><span data-stu-id="43142-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="43142-126">Permitir que todos os aplicativos de cliente para usar o EWS exceto aqueles especificamente bloqueados.</span><span class="sxs-lookup"><span data-stu-id="43142-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="43142-127">Este exemplo bloqueia somente de aplicativos usando o EWS que possuem uma cadeia de caracteres de agente de usuário que inicia com "OWA /".</span><span class="sxs-lookup"><span data-stu-id="43142-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="43142-128">Permitir que todos os aplicativos de cliente para usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="43142-129">Porque nenhuma lista de bloqueios for especificada, todos os aplicativos podem usar EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="43142-130">Bloquear toda a organização utilizem EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="43142-131">Permitir que toda a organização usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="43142-132">Bloquear uma caixa de correio individual do usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="43142-133">Permitir que uma caixa de correio individual usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="43142-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="43142-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="43142-134">See also</span></span>

- [<span data-ttu-id="43142-135">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="43142-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="43142-136">Controlando o acesso do aplicativo de cliente para o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43142-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="43142-137">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="43142-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="43142-138">O Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="43142-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

