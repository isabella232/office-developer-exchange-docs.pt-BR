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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455895"
---
# <a name="configure-impersonation"></a>Configurar representação

Saiba como conceder a função de representação a uma conta de serviço usando o Shell de gerenciamento do Exchange. 
  
A representação permite que um chamador, como um aplicativo de serviço, represente uma conta de usuário. O chamador pode executar operações usando as permissões associadas à conta representada em vez das permissões associadas à conta do chamador.
  
O Exchange Online, o Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013 usam o controle de acesso baseado em função (RBAC) para atribuir permissões a contas. O administrador do Exchange Server precisará conceder a qualquer conta de serviço que irá representar outros usuários a função **ApplicationImpersonation** usando o cmdlet [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) . 
  
## <a name="configuring-the-applicationimpersonation-role"></a>Configurando a função ApplicationImpersonation

Quando você ou seu administrador de servidor do Exchanger atribui a função **ApplicationImpersonation** , use os seguintes parâmetros do cmdlet **New-ManagementRoleAssignment** : 
  
-  _Nome_ &ndash; O nome amigável da atribuição de função. Cada vez que você atribui uma função, uma entrada é feita na lista de funções RBAC. Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
    
-  _Função_ &ndash; A função RBAC a ser atribuída. Ao configurar a representação, você atribui a função **ApplicationImpersonation** . 
    
-  _Usuário_ &ndash; A conta de serviço. 
    
-  _CustomRecipientScope_ &ndash; O escopo de usuários que a conta de serviço pode representar. A conta de serviço só poderá representar outros usuários dentro do escopo especificado. Se nenhum escopo for especificado, a conta de serviço receberá a função **ApplicationImpersonation** sobre todos os usuários em uma organização. Você pode criar escopos de gerenciamento personalizados usando o cmdlet [New-ManagementScope](https://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) . 
    
Antes de poder configurar a representação, você precisa:
  
- Credenciais administrativas para o Exchange Server.
    
- Credenciais de administrador de domínio ou outras credenciais com permissão para criar e atribuir funções e escopos.
    
- Ferramentas de gerenciamento do Exchange. Eles são instalados no computador a partir do qual os comandos serão executados.
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>Para configurar a representação para todos os usuários em uma organização

1. Abra o Shell de Gerenciamento do Exchange Management Shell. No menu Iniciar, escolha **todos os programas**  >  **Microsoft Exchange Server 2013**. 
    
2. Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão de representação ao usuário especificado. O exemplo a seguir mostra como configurar a representação para habilitar uma conta de serviço para representar todos os outros usuários em uma organização. 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>Para configurar a representação de usuários específicos ou grupos de usuários

1. Abra o Shell de Gerenciamento do Exchange Management Shell. No menu Iniciar, escolha **todos os programas**  >  **Microsoft Exchange Server 2013**. 
    
2. Execute o cmdlet **New-ManagementScope** para criar um escopo para o qual a função de representação pode ser atribuída. Se um escopo existente estiver disponível, você poderá pular esta etapa. O exemplo a seguir mostra como criar um escopo de gerenciamento para um grupo específico. 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   O parâmetro _RecipientRestrictionFilter_ do cmdlet **New-ManagementScope** define os membros do escopo. Você pode usar as propriedades do objeto **Identity** para criar o filtro. O exemplo a seguir é um filtro que restringe o resultado para um único usuário com o nome de usuário "João". 
    
   ```powershell
   Name -eq "john"
   ```

3. Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão para representar os membros do escopo especificado. O exemplo a seguir mostra como configurar uma conta de serviço para representar todos os usuários em um escopo. 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


Depois que o administrador conceder permissões de representação, você poderá usar a conta de serviço para fazer chamadas com as contas de outros usuários. Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
  
## <a name="see-also"></a>Confira também

- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
- [Função ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment](https://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](https://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

