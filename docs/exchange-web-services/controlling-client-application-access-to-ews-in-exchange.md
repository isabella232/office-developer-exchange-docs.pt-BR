---
title: Controlando o acesso do aplicativo de cliente para o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Saiba mais sobre as opções para gerenciar o acesso do aplicativo cliente para o EWS.
ms.openlocfilehash: e3a0e07b733b4ebc070ab6b3fc73c8aec4b62785
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353060"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="60609-103">Controlando o acesso do aplicativo de cliente para o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="60609-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="60609-104">Saiba mais sobre as opções para gerenciar o acesso do aplicativo cliente para o EWS.</span><span class="sxs-lookup"><span data-stu-id="60609-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="60609-105">Qualquer aplicativo de cliente do EWS que você criar deve ter acesso concedido ao Exchange Online, Exchange Online como parte do Office 365 ou a versão do Exchange começando com o Exchange 2013 antes que ele possa chamar operações do EWS.</span><span class="sxs-lookup"><span data-stu-id="60609-105">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations.</span></span> <span data-ttu-id="60609-106">Administradores de servidor de teste ou de produção podem usar o Shell de gerenciamento do Exchange para limitar o acesso aos EWS para todos os usuários e aplicativos, para usuários individuais ou para aplicativos individuais.</span><span class="sxs-lookup"><span data-stu-id="60609-106">Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications.</span></span> <span data-ttu-id="60609-107">Controle de acesso para o EWS baseia-se em contas de domínio.</span><span class="sxs-lookup"><span data-stu-id="60609-107">Access control for EWS is based on domain accounts.</span></span> <span data-ttu-id="60609-108">Quando uma conexão é feita com credenciais que são autenticadas pela autoridade de segurança local, o servidor retornará um erro que indica que somente contas de domínio podem se conectar.</span><span class="sxs-lookup"><span data-stu-id="60609-108">When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="60609-109">Controle de acesso para clientes do EWS e usuários</span><span class="sxs-lookup"><span data-stu-id="60609-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="60609-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="60609-110"></span></span>

<span data-ttu-id="60609-111">O administrador do servidor de teste ou de produção pode configurar o controle de acesso para clientes que se conectam ao EWS das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="60609-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="60609-112">Impedindo que todos os aplicativos de cliente de se conectar.</span><span class="sxs-lookup"><span data-stu-id="60609-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="60609-113">Permitindo o cliente específico aplicativos apenas para se conectar.</span><span class="sxs-lookup"><span data-stu-id="60609-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="60609-114">Permitindo a qualquer aplicativo cliente para se conectar, exceto aqueles especificamente bloqueados.</span><span class="sxs-lookup"><span data-stu-id="60609-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="60609-115">Permitindo a qualquer aplicativo cliente para se conectar.</span><span class="sxs-lookup"><span data-stu-id="60609-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="60609-116">Aplicativos são identificados pela cadeia de caracteres de agente de usuário que enviam na solicitação HTTP web.</span><span class="sxs-lookup"><span data-stu-id="60609-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="60609-117">Bloqueio de nível de aplicativo não é um recurso de segurança.</span><span class="sxs-lookup"><span data-stu-id="60609-117">Application-level blocking is not a security feature.</span></span> <span data-ttu-id="60609-118">A cadeia de caracteres de agente do usuário é falsificada facilmente.</span><span class="sxs-lookup"><span data-stu-id="60609-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="60609-119">Se um aplicativo tem acesso permitido ao EWS, o aplicativo deve ainda apresentar credenciais que o servidor autenticar antes que o aplicativo pode se conectar ao EWS.</span><span class="sxs-lookup"><span data-stu-id="60609-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="60609-120">Os administradores também podem configurar o controle de acesso para proprietários de caixa de correio que se conectam ao EWS das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="60609-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="60609-121">Bloqueando ou permitindo que uma organização inteira.</span><span class="sxs-lookup"><span data-stu-id="60609-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="60609-122">Bloqueando ou permitindo que um grupo de usuários identificado por um escopo de autenticação baseada em função que inclui ou exclui os proprietários de caixa de correio que não têm acesso ao EWS.</span><span class="sxs-lookup"><span data-stu-id="60609-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="60609-123">Bloqueando ou permitindo que um proprietário de caixa de correio individuais.</span><span class="sxs-lookup"><span data-stu-id="60609-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="60609-124">Configurações de controle de acesso específicos substituem configurações de controle de acesso geral.</span><span class="sxs-lookup"><span data-stu-id="60609-124">Specific access control settings override general access control settings.</span></span> <span data-ttu-id="60609-125">Por exemplo, se uma organização negue acesso EWS, mas um proprietário de caixa de correio individual tem permissão de acesso de aplicativo, a configuração individual prevalecerá e acesso é permitido.</span><span class="sxs-lookup"><span data-stu-id="60609-125">For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="60609-126">Gerenciamento de acesso do EWS e delegação</span><span class="sxs-lookup"><span data-stu-id="60609-126">Delegation and EWS access management</span></span>
<span data-ttu-id="60609-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="60609-127"></span></span>

<span data-ttu-id="60609-128">Quando o representante de usuários que não têm acesso ao EWS usar seu aplicativo de cliente, eles não poderão acessar a caixa de correio do usuário principal usando EWS, mesmo se o usuário principal tem EWS acessar.</span><span class="sxs-lookup"><span data-stu-id="60609-128">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access.</span></span> <span data-ttu-id="60609-129">Se o usuário delegado tem acesso EWS, o representante será capaz de usar seu aplicativo de cliente do EWS para acessar a caixa de correio do usuário principal, mesmo se o usuário principal EWS não tem acesso.</span><span class="sxs-lookup"><span data-stu-id="60609-129">If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="60609-130">Representação e gerenciamento de acesso EWS</span><span class="sxs-lookup"><span data-stu-id="60609-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="60609-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="60609-131"></span></span>

<span data-ttu-id="60609-132">Aplicativos cliente que se conectam ao EWS em nome de proprietários de caixa de correio podem não ser capazes de usar as configurações do EWS do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60609-132">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner.</span></span> <span data-ttu-id="60609-133">Por exemplo, um aplicativo que arquiva mensagens são para uma empresa tem para se conectar ao EWS independentemente das configurações de que a caixa de correio dos usuários de email.</span><span class="sxs-lookup"><span data-stu-id="60609-133">For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are.</span></span> <span data-ttu-id="60609-134">Outros aplicativos, como clientes de email, é necessário usar as configurações do EWS do proprietário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60609-134">Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="60609-135">Os administradores devem criar uma conta de representação para cada aplicativo ou classe de aplicativos que eles usam no seu servidor.</span><span class="sxs-lookup"><span data-stu-id="60609-135">Administrators should create an impersonation account for each application or application class that they use on their server.</span></span> <span data-ttu-id="60609-136">Isso permitirá que o administrador configure o escopo de controle de acesso baseado em função para todos os usuários que não possui permissões de EWS.</span><span class="sxs-lookup"><span data-stu-id="60609-136">This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="60609-137">Para habilitar contas de representação, o administrador do servidor de teste ou de produção deve siga um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="60609-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="60609-138">Adicione o grupo de usuários autenticados ao grupo acesso compatível pré-Win2K.</span><span class="sxs-lookup"><span data-stu-id="60609-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="60609-139">Adicione o grupo de servidores do Exchange ao grupo de acesso de autorização do Windows.</span><span class="sxs-lookup"><span data-stu-id="60609-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="60609-140">Cmdlets do Shell de gerenciamento do Exchange para o gerenciamento de acesso</span><span class="sxs-lookup"><span data-stu-id="60609-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="60609-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="60609-141"></span></span>

<span data-ttu-id="60609-142">Os administradores usar os seguintes cmdlets do Shell de gerenciamento do Exchange para configurar os controles de acesso do EWS:</span><span class="sxs-lookup"><span data-stu-id="60609-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="60609-143">Get-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="60609-143">Get-CASMailbox</span></span>](http://technet.microsoft.com/en-us/library/bb124754.aspx)   
- [<span data-ttu-id="60609-144">Set-CASMailbox</span><span class="sxs-lookup"><span data-stu-id="60609-144">Set-CASMailbox</span></span>](http://technet.microsoft.com/en-us/library/bb125264.aspx)   
- [<span data-ttu-id="60609-145">Get-OrganizationConfig.</span><span class="sxs-lookup"><span data-stu-id="60609-145">Get-OrganizationConfig</span></span>](http://technet.microsoft.com/en-us/library/aa997571.aspx)   
- [<span data-ttu-id="60609-146">Set-OrganizationConfig.</span><span class="sxs-lookup"><span data-stu-id="60609-146">Set-OrganizationConfig</span></span>](http://technet.microsoft.com/en-us/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="60609-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="60609-147">See also</span></span>

- [<span data-ttu-id="60609-148">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="60609-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="60609-149">Controlar o acesso a EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="60609-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="60609-150">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="60609-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="60609-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="60609-151">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

