---
title: Configurar representação
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Aprenda a conceder o papel de representação para uma conta de serviço usando o Shell de gerenciamento do Exchange.
ms.openlocfilehash: 57ccef48a7553bcc06e3b3ae940b376b8555ef84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750701"
---
# <a name="configure-impersonation"></a><span data-ttu-id="9ad08-103">Configurar representação</span><span class="sxs-lookup"><span data-stu-id="9ad08-103">Configure impersonation</span></span>

<span data-ttu-id="9ad08-104">Aprenda a conceder o papel de representação para uma conta de serviço usando o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ad08-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="9ad08-105">Representação permite que um chamador, como um aplicativo de serviço, para representar uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="9ad08-105">Impersonation enables a caller, such as a service application, to impersonate a user account.</span></span> <span data-ttu-id="9ad08-106">O chamador pode executar operações usando as permissões que estão associadas a conta representada em vez de permissões associadas a conta do chamador.</span><span class="sxs-lookup"><span data-stu-id="9ad08-106">The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="9ad08-107">O Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013 use o controle de acesso baseado em função (RBAC) para atribuir permissões a contas.</span><span class="sxs-lookup"><span data-stu-id="9ad08-107">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts.</span></span> <span data-ttu-id="9ad08-108">O administrador do servidor Exchange precisará conceder a função **ApplicationImpersonation** de qualquer conta de serviço que vai ser representando a outros usuários usando o cmdlet [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9ad08-108">Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="9ad08-109">Configurando a função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="9ad08-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="9ad08-110">Quando você ou o administrador do servidor Exchanger atribui a função **ApplicationImpersonation** , use os seguintes parâmetros do cmdlet **New-ManagementRoleAssignment** :</span><span class="sxs-lookup"><span data-stu-id="9ad08-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="9ad08-111">_Nome_ &ndash; o nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9ad08-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="9ad08-112">Cada vez que você atribuir uma função, será feita uma entrada na lista de funções de RBAC.</span><span class="sxs-lookup"><span data-stu-id="9ad08-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="9ad08-113">Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9ad08-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="9ad08-114">_Função_ &ndash; Função de RBAC a atribuir.</span><span class="sxs-lookup"><span data-stu-id="9ad08-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="9ad08-115">Quando você configura a representação, você pode atribuir a função **ApplicationImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="9ad08-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="9ad08-116">_Usuário_ &ndash; a conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="9ad08-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="9ad08-117">_CustomRecipientScope_ &ndash; o escopo de usuários que pode representar a conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="9ad08-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="9ad08-118">A conta de serviço somente poderão se passem por outros usuários dentro do escopo especificado.</span><span class="sxs-lookup"><span data-stu-id="9ad08-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="9ad08-119">Se nenhum escopo for especificado, a conta de serviço recebe a função **ApplicationImpersonation** sobre todos os usuários em uma organização.</span><span class="sxs-lookup"><span data-stu-id="9ad08-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="9ad08-120">Você pode criar escopos de gerenciamento personalizado usando o cmdlet [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9ad08-120">You can create custom management scopes by using the [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="9ad08-121">Antes de você poder configurar representação, você precisa:</span><span class="sxs-lookup"><span data-stu-id="9ad08-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="9ad08-122">Credenciais administrativas para o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="9ad08-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="9ad08-123">Credenciais de administrador de domínio ou outras credenciais com a permissão para criar e atribuir funções e escopos.</span><span class="sxs-lookup"><span data-stu-id="9ad08-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="9ad08-124">Ferramentas de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ad08-124">Exchange management tools.</span></span> <span data-ttu-id="9ad08-125">Eles são instalados no computador do qual você executará os comandos.</span><span class="sxs-lookup"><span data-stu-id="9ad08-125">These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="9ad08-126">Para configurar a representação para todos os usuários em uma organização</span><span class="sxs-lookup"><span data-stu-id="9ad08-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="9ad08-127">Abra o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ad08-127">Open the Exchange Management Shell.</span></span> <span data-ttu-id="9ad08-128">No menu Iniciar, escolha **Todos os programas** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="9ad08-128">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="9ad08-129">Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão de representação ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="9ad08-129">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user.</span></span> <span data-ttu-id="9ad08-130">O exemplo a seguir mostra como configurar a representação para habilitar uma conta de serviço representar todos os outros usuários em uma organização.</span><span class="sxs-lookup"><span data-stu-id="9ad08-130">The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="9ad08-131">Para configurar a representação para usuários específicos ou grupos de usuários</span><span class="sxs-lookup"><span data-stu-id="9ad08-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="9ad08-132">Abra o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ad08-132">Open the Exchange Management Shell.</span></span> <span data-ttu-id="9ad08-133">No menu Iniciar, escolha **Todos os programas** > **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="9ad08-133">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="9ad08-134">Execute o cmdlet **New-ManagementScope** para criar um escopo ao qual a função de representação pode ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="9ad08-134">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned.</span></span> <span data-ttu-id="9ad08-135">Se um escopo existente estiver disponível, você poderá ignorar esta etapa.</span><span class="sxs-lookup"><span data-stu-id="9ad08-135">If an existing scope is available, you can skip this step.</span></span> <span data-ttu-id="9ad08-136">O exemplo a seguir mostra como criar um escopo de gerenciamento de um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="9ad08-136">The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="9ad08-137">O parâmetro _RecipientRestrictionFilter_ do cmdlet **New-ManagementScope** define os membros do escopo.</span><span class="sxs-lookup"><span data-stu-id="9ad08-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="9ad08-138">Você pode usar as propriedades do objeto de **identidade** para criar o filtro.</span><span class="sxs-lookup"><span data-stu-id="9ad08-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="9ad08-139">O exemplo a seguir é um filtro que restringe o resultado para um único usuário com o usuário nome "João".</span><span class="sxs-lookup"><span data-stu-id="9ad08-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="9ad08-140">Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão para representar os membros do escopo especificado.</span><span class="sxs-lookup"><span data-stu-id="9ad08-140">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope.</span></span> <span data-ttu-id="9ad08-141">O exemplo a seguir mostra como configurar uma conta de serviço para representar todos os usuários em um escopo.</span><span class="sxs-lookup"><span data-stu-id="9ad08-141">The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="9ad08-142">Depois que o administrador concede permissões de representação, você pode usar a conta de serviço para fazer chamadas contra contas de outros usuários.</span><span class="sxs-lookup"><span data-stu-id="9ad08-142">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts.</span></span> <span data-ttu-id="9ad08-143">Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9ad08-143">You can verify role assignments by using the [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9ad08-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="9ad08-144">See also</span></span>

- [<span data-ttu-id="9ad08-145">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9ad08-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="9ad08-146">Função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="9ad08-146">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="9ad08-147">New-ManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="9ad08-147">New-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="9ad08-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9ad08-148">Get-ManagementRoleAssignment</span></span>](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

