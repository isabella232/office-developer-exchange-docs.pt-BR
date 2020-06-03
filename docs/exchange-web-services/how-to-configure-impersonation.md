---
title: Configurar representação
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: efcef39f-e26d-4eed-95ac-36a5bf8c089f
description: Saiba como conceder a função de representação a uma conta de serviço usando o Shell de gerenciamento do Exchange.
localization_priority: Priority
ms.openlocfilehash: f8fe95536213e347840af082d765a9cc2fbce819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455895"
---
# <a name="configure-impersonation"></a><span data-ttu-id="21830-103">Configurar representação</span><span class="sxs-lookup"><span data-stu-id="21830-103">Configure impersonation</span></span>

<span data-ttu-id="21830-104">Saiba como conceder a função de representação a uma conta de serviço usando o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="21830-104">Learn how to grant the impersonation role to a service account by using the Exchange Management Shell.</span></span> 
  
<span data-ttu-id="21830-105">A representação permite que um chamador, como um aplicativo de serviço, represente uma conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="21830-105">Impersonation enables a caller, such as a service application, to impersonate a user account.</span></span> <span data-ttu-id="21830-106">O chamador pode executar operações usando as permissões associadas à conta representada em vez das permissões associadas à conta do chamador.</span><span class="sxs-lookup"><span data-stu-id="21830-106">The caller can perform operations by using the permissions that are associated with the impersonated account instead of the permissions associated with the caller's account.</span></span>
  
<span data-ttu-id="21830-107">O Exchange Online, o Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013 usam o controle de acesso baseado em função (RBAC) para atribuir permissões a contas.</span><span class="sxs-lookup"><span data-stu-id="21830-107">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013 use role-based access control (RBAC) to assign permissions to accounts.</span></span> <span data-ttu-id="21830-108">O administrador do Exchange Server precisará conceder a qualquer conta de serviço que irá representar outros usuários a função **ApplicationImpersonation** usando o cmdlet [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) .</span><span class="sxs-lookup"><span data-stu-id="21830-108">Your Exchange server administrator will need to grant any service account that will be impersonating other users the **ApplicationImpersonation** role by using the [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) cmdlet.</span></span> 
  
## <a name="configuring-the-applicationimpersonation-role"></a><span data-ttu-id="21830-109">Configurando a função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="21830-109">Configuring the ApplicationImpersonation role</span></span>

<span data-ttu-id="21830-110">Quando você ou seu administrador de servidor do Exchanger atribui a função **ApplicationImpersonation** , use os seguintes parâmetros do cmdlet **New-ManagementRoleAssignment** :</span><span class="sxs-lookup"><span data-stu-id="21830-110">When you or your Exchanger server administrator assigns the **ApplicationImpersonation** role, use the following parameters of the **New-ManagementRoleAssignment** cmdlet:</span></span> 
  
-  <span data-ttu-id="21830-111">_Nome_ &ndash; O nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="21830-111">_Name_ &ndash; The friendly name of the role assignment.</span></span> <span data-ttu-id="21830-112">Cada vez que você atribui uma função, uma entrada é feita na lista de funções RBAC.</span><span class="sxs-lookup"><span data-stu-id="21830-112">Each time that you assign a role, an entry is made in the RBAC roles list.</span></span> <span data-ttu-id="21830-113">Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="21830-113">You can verify role assignments by using the [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
    
-  <span data-ttu-id="21830-114">_Função_ &ndash; A função RBAC a ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="21830-114">_Role_ &ndash; The RBAC role to assign.</span></span> <span data-ttu-id="21830-115">Ao configurar a representação, você atribui a função **ApplicationImpersonation** .</span><span class="sxs-lookup"><span data-stu-id="21830-115">When you set up impersonation, you assign the **ApplicationImpersonation** role.</span></span> 
    
-  <span data-ttu-id="21830-116">_Usuário_ &ndash; A conta de serviço.</span><span class="sxs-lookup"><span data-stu-id="21830-116">_User_ &ndash; The service account.</span></span> 
    
-  <span data-ttu-id="21830-117">_CustomRecipientScope_ &ndash; O escopo de usuários que a conta de serviço pode representar.</span><span class="sxs-lookup"><span data-stu-id="21830-117">_CustomRecipientScope_ &ndash; The scope of users that the service account can impersonate.</span></span> <span data-ttu-id="21830-118">A conta de serviço só poderá representar outros usuários dentro do escopo especificado.</span><span class="sxs-lookup"><span data-stu-id="21830-118">The service account will only be allowed to impersonate other users within the specified scope.</span></span> <span data-ttu-id="21830-119">Se nenhum escopo for especificado, a conta de serviço receberá a função **ApplicationImpersonation** sobre todos os usuários em uma organização.</span><span class="sxs-lookup"><span data-stu-id="21830-119">If no scope is specified, the service account is granted the **ApplicationImpersonation** role over all users in an organization.</span></span> <span data-ttu-id="21830-120">Você pode criar escopos de gerenciamento personalizados usando o cmdlet [New-ManagementScope](https://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) .</span><span class="sxs-lookup"><span data-stu-id="21830-120">You can create custom management scopes by using the [New-ManagementScope](https://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) cmdlet.</span></span> 
    
<span data-ttu-id="21830-121">Antes de poder configurar a representação, você precisa:</span><span class="sxs-lookup"><span data-stu-id="21830-121">Before you can configure impersonation, you need:</span></span>
  
- <span data-ttu-id="21830-122">Credenciais administrativas para o Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="21830-122">Administrative credentials for the Exchange server.</span></span>
    
- <span data-ttu-id="21830-123">Credenciais de administrador de domínio ou outras credenciais com permissão para criar e atribuir funções e escopos.</span><span class="sxs-lookup"><span data-stu-id="21830-123">Domain Administrator credentials, or other credentials with the permission to create and assign roles and scopes.</span></span>
    
- <span data-ttu-id="21830-124">Ferramentas de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="21830-124">Exchange management tools.</span></span> <span data-ttu-id="21830-125">Eles são instalados no computador a partir do qual os comandos serão executados.</span><span class="sxs-lookup"><span data-stu-id="21830-125">These are installed on the computer from which you will run the commands.</span></span>
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a><span data-ttu-id="21830-126">Para configurar a representação para todos os usuários em uma organização</span><span class="sxs-lookup"><span data-stu-id="21830-126">To configure impersonation for all users in an organization</span></span>

1. <span data-ttu-id="21830-127">Abra o Shell de Gerenciamento do Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="21830-127">Open the Exchange Management Shell.</span></span> <span data-ttu-id="21830-128">No menu Iniciar, escolha **todos os programas**  >  **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="21830-128">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="21830-129">Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão de representação ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="21830-129">Run the **New-ManagementRoleAssignment** cmdlet to add the impersonation permission to the specified user.</span></span> <span data-ttu-id="21830-130">O exemplo a seguir mostra como configurar a representação para habilitar uma conta de serviço para representar todos os outros usuários em uma organização.</span><span class="sxs-lookup"><span data-stu-id="21830-130">The following example shows how to configure impersonation to enable a service account to impersonate all other users in an organization.</span></span> 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a><span data-ttu-id="21830-131">Para configurar a representação de usuários específicos ou grupos de usuários</span><span class="sxs-lookup"><span data-stu-id="21830-131">To configure impersonation for specific users or groups of users</span></span>

1. <span data-ttu-id="21830-132">Abra o Shell de Gerenciamento do Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="21830-132">Open the Exchange Management Shell.</span></span> <span data-ttu-id="21830-133">No menu Iniciar, escolha **todos os programas**  >  **Microsoft Exchange Server 2013**.</span><span class="sxs-lookup"><span data-stu-id="21830-133">From the Start menu, choose **All Programs** > **Microsoft Exchange Server 2013**.</span></span> 
    
2. <span data-ttu-id="21830-134">Execute o cmdlet **New-ManagementScope** para criar um escopo para o qual a função de representação pode ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="21830-134">Run the **New-ManagementScope** cmdlet to create a scope to which the impersonation role can be assigned.</span></span> <span data-ttu-id="21830-135">Se um escopo existente estiver disponível, você poderá pular esta etapa.</span><span class="sxs-lookup"><span data-stu-id="21830-135">If an existing scope is available, you can skip this step.</span></span> <span data-ttu-id="21830-136">O exemplo a seguir mostra como criar um escopo de gerenciamento para um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="21830-136">The following example shows how to create a management scope for a specific group.</span></span> 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   <span data-ttu-id="21830-137">O parâmetro _RecipientRestrictionFilter_ do cmdlet **New-ManagementScope** define os membros do escopo.</span><span class="sxs-lookup"><span data-stu-id="21830-137">The _RecipientRestrictionFilter_ parameter of the **New-ManagementScope** cmdlet defines the members of the scope.</span></span> <span data-ttu-id="21830-138">Você pode usar as propriedades do objeto **Identity** para criar o filtro.</span><span class="sxs-lookup"><span data-stu-id="21830-138">You can use the properties of the **Identity** object to create the filter.</span></span> <span data-ttu-id="21830-139">O exemplo a seguir é um filtro que restringe o resultado para um único usuário com o nome de usuário "João".</span><span class="sxs-lookup"><span data-stu-id="21830-139">The following example is a filter that restricts the result to a single user with the user name "john."</span></span> 
    
   ```powershell
   Name -eq "john"
   ```

3. <span data-ttu-id="21830-140">Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão para representar os membros do escopo especificado.</span><span class="sxs-lookup"><span data-stu-id="21830-140">Run the **New-ManagementRoleAssignment** cmdlet to add the permission to impersonate the members of the specified scope.</span></span> <span data-ttu-id="21830-141">O exemplo a seguir mostra como configurar uma conta de serviço para representar todos os usuários em um escopo.</span><span class="sxs-lookup"><span data-stu-id="21830-141">The following example shows how to configure a service account to impersonate all users in a scope.</span></span> 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


<span data-ttu-id="21830-142">Depois que o administrador conceder permissões de representação, você poderá usar a conta de serviço para fazer chamadas com as contas de outros usuários.</span><span class="sxs-lookup"><span data-stu-id="21830-142">After your administrator grants impersonation permissions, you can use the service account to make calls against other users' accounts.</span></span> <span data-ttu-id="21830-143">Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) .</span><span class="sxs-lookup"><span data-stu-id="21830-143">You can verify role assignments by using the [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) cmdlet.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="21830-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="21830-144">See also</span></span>

- [<span data-ttu-id="21830-145">Representação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="21830-145">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
- [<span data-ttu-id="21830-146">Função ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="21830-146">ApplicationImpersonation role</span></span>](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="21830-147">New-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="21830-147">New-ManagementRoleAssignment</span></span>](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [<span data-ttu-id="21830-148">Get-ManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="21830-148">Get-ManagementRoleAssignment</span></span>](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

