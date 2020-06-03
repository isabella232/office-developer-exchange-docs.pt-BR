---
title: Controlando o acesso do aplicativo cliente ao EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Saiba mais sobre as opções para gerenciar o acesso de aplicativos cliente ao EWS.
localization_priority: Priority
ms.openlocfilehash: b887b8167e3d38946b1d6caffe12655ded89569f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528458"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="de797-103">Controlando o acesso do aplicativo cliente ao EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de797-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="de797-104">Saiba mais sobre as opções para gerenciar o acesso de aplicativos cliente ao EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="de797-105">Qualquer aplicativo cliente do EWS que você criar deve ter acesso ao Exchange Online, ao Exchange Online como parte do Office 365, ou a versão do Exchange a partir do Exchange 2013, antes de poder chamar as operações do EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="de797-106">Os administradores do servidor de teste ou de produção podem usar o Shell de gerenciamento do Exchange para limitar o acesso ao EWS para todos os usuários e aplicativos, para usuários individuais ou para aplicativos individuais.</span><span class="sxs-lookup"><span data-stu-id="de797-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="de797-107">O controle de acesso para EWS é baseado em contas de domínio.</span><span class="sxs-lookup"><span data-stu-id="de797-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="de797-108">Quando uma conexão é feita com credenciais autenticadas pela autoridade de segurança local, o servidor retorna um erro que indica que somente as contas de domínio podem se conectar.</span><span class="sxs-lookup"><span data-stu-id="de797-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="de797-109">Controle de acesso para clientes e usuários do EWS</span><span class="sxs-lookup"><span data-stu-id="de797-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="de797-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="de797-110"><a name="bk_configure"> </a></span></span>

<span data-ttu-id="de797-111">Seu administrador de teste ou de servidor de produção pode configurar o controle de acesso para clientes que se conectam ao EWS das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="de797-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="de797-112">Bloqueando a conexão de todos os aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="de797-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="de797-113">Permitindo que aplicativos clientes específicos apenas se conectem.</span><span class="sxs-lookup"><span data-stu-id="de797-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="de797-114">Permitindo que qualquer aplicativo cliente se conecte, exceto aqueles especificamente bloqueados.</span><span class="sxs-lookup"><span data-stu-id="de797-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="de797-115">Permitindo que qualquer aplicativo cliente se conecte.</span><span class="sxs-lookup"><span data-stu-id="de797-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="de797-116">Os aplicativos são identificados pela cadeia de caracteres do agente de usuário que eles enviam na solicitação HTTP Web.</span><span class="sxs-lookup"><span data-stu-id="de797-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="de797-117">O bloqueio no nível do aplicativo não é um recurso de segurança.</span><span class="sxs-lookup"><span data-stu-id="de797-117">Application-level blocking is not a security feature.</span></span> <span data-ttu-id="de797-118">A cadeia de caracteres do agente do usuário é facilmente falsificada.</span><span class="sxs-lookup"><span data-stu-id="de797-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="de797-119">Se um aplicativo tiver acesso ao EWS, o aplicativo ainda deverá apresentar as credenciais que o servidor autentica para que o aplicativo possa se conectar ao EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="de797-120">Os administradores também podem configurar o controle de acesso para proprietários de caixa de correio que se conectam ao EWS das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="de797-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="de797-121">Bloqueando ou permitindo uma organização inteira.</span><span class="sxs-lookup"><span data-stu-id="de797-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="de797-122">Bloqueando ou permitindo um grupo de usuários identificado por um escopo de autenticação baseada em função que inclui ou exclui proprietários de caixa de correio que não têm acesso ao EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="de797-123">Bloqueando ou permitindo um proprietário de caixa de correio individual.</span><span class="sxs-lookup"><span data-stu-id="de797-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="de797-124">As configurações de controle de acesso específicas substituem as configurações de controle de acesso gerais.</span><span class="sxs-lookup"><span data-stu-id="de797-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="de797-125">Por exemplo, se uma organização negar acesso ao EWS, mas um proprietário de caixa de correio individual tiver permissão de acesso de aplicativo, a configuração individual prevalecerá e o acesso será permitido.</span><span class="sxs-lookup"><span data-stu-id="de797-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="de797-126">Gerenciamento de delegação e acesso de EWS</span><span class="sxs-lookup"><span data-stu-id="de797-126">Delegation and EWS access management</span></span>
<span data-ttu-id="de797-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="de797-127"><a name="bk_delegation"> </a></span></span>

<span data-ttu-id="de797-128">Quando os usuários delegados que não têm acesso ao EWS usam seu aplicativo cliente, eles não poderão acessar a caixa de correio do usuário principal usando o EWS, mesmo que o usuário principal tenha acesso EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="de797-129">Se o usuário delegado tiver acesso EWS, o representante será capaz de usar seu aplicativo cliente do EWS para acessar a caixa de correio do usuário principal, mesmo que o usuário principal não tenha acesso EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="de797-130">Gerenciamento de acesso e representação do EWS</span><span class="sxs-lookup"><span data-stu-id="de797-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="de797-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="de797-131"><a name="bk_impersonation"> </a></span></span>

<span data-ttu-id="de797-132">Os aplicativos cliente que se conectam ao EWS em nome dos proprietários da caixa de correio podem não conseguir usar as configurações do EWS do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="de797-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="de797-133">Por exemplo, um aplicativo que arquiva mensagens de email de uma empresa deve se conectar ao EWS independentemente das configurações de caixa de correio dos usuários.</span><span class="sxs-lookup"><span data-stu-id="de797-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="de797-134">Outros aplicativos, como clientes de email, precisam usar as configurações do EWS do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="de797-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="de797-135">Os administradores devem criar uma conta de representação para cada aplicativo ou classe de aplicativo que eles usam no servidor.</span><span class="sxs-lookup"><span data-stu-id="de797-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="de797-136">Isso permitirá que o administrador configure o escopo de controle de acesso baseado em função para todos os usuários que não têm permissões de EWS.</span><span class="sxs-lookup"><span data-stu-id="de797-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="de797-137">Para habilitar as contas de representação, seu administrador de teste ou de servidor de produção deve executar uma das seguintes ações:</span><span class="sxs-lookup"><span data-stu-id="de797-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="de797-138">Adicione o grupo usuários autenticados ao grupo acesso compatível com o anterior ao Win2K.</span><span class="sxs-lookup"><span data-stu-id="de797-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="de797-139">Adicione o grupo Exchange Servers ao grupo de acesso de autorização do Windows.</span><span class="sxs-lookup"><span data-stu-id="de797-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="de797-140">Cmdlets do Shell de gerenciamento do Exchange para gerenciamento de acesso</span><span class="sxs-lookup"><span data-stu-id="de797-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="de797-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="de797-141"><a name="bk_cmdlets"> </a></span></span>

<span data-ttu-id="de797-142">Os administradores usam os seguintes cmdlets do Shell de gerenciamento do Exchange para configurar os controles de acesso do EWS:</span><span class="sxs-lookup"><span data-stu-id="de797-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="de797-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="de797-143">Get-CASMailbox</span></span>](https://technet.microsoft.com/library/bb124754.aspx)   
- [<span data-ttu-id="de797-144">Set-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="de797-144">Set-CASMailbox</span></span>](https://technet.microsoft.com/library/bb125264.aspx)   
- [<span data-ttu-id="de797-145">Get-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="de797-145">Get-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997571.aspx)   
- [<span data-ttu-id="de797-146">Set-OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="de797-146">Set-OrganizationConfig</span></span>](https://technet.microsoft.com/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="de797-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="de797-147">See also</span></span>

- [<span data-ttu-id="de797-148">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="de797-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="de797-149">Controlar o acesso ao EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de797-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="de797-150">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="de797-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="de797-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="de797-151">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

