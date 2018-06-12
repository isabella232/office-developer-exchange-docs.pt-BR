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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750701"
---
# <a name="configure-impersonation"></a>Configurar representação

Aprenda a conceder o papel de representação para uma conta de serviço usando o Shell de gerenciamento do Exchange. 
  
Representação permite que um chamador, como um aplicativo de serviço, para representar uma conta de usuário. O chamador pode executar operações usando as permissões que estão associadas a conta representada em vez de permissões associadas a conta do chamador.
  
O Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013 use o controle de acesso baseado em função (RBAC) para atribuir permissões a contas. O administrador do servidor Exchange precisará conceder a função **ApplicationImpersonation** de qualquer conta de serviço que vai ser representando a outros usuários usando o cmdlet [New-ManagementRoleAssignment](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx) . 
  
## <a name="configuring-the-applicationimpersonation-role"></a>Configurando a função ApplicationImpersonation

Quando você ou o administrador do servidor Exchanger atribui a função **ApplicationImpersonation** , use os seguintes parâmetros do cmdlet **New-ManagementRoleAssignment** : 
  
-  _Nome_ &ndash; o nome amigável da atribuição de função. Cada vez que você atribuir uma função, será feita uma entrada na lista de funções de RBAC. Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
    
-  _Função_ &ndash; Função de RBAC a atribuir. Quando você configura a representação, você pode atribuir a função **ApplicationImpersonation** . 
    
-  _Usuário_ &ndash; a conta de serviço. 
    
-  _CustomRecipientScope_ &ndash; o escopo de usuários que pode representar a conta de serviço. A conta de serviço somente poderão se passem por outros usuários dentro do escopo especificado. Se nenhum escopo for especificado, a conta de serviço recebe a função **ApplicationImpersonation** sobre todos os usuários em uma organização. Você pode criar escopos de gerenciamento personalizado usando o cmdlet [New-ManagementScope](http://msdn.microsoft.com/library/1ea1f474-69d6-48c0-9beb-bfa4442c5dab.aspx) . 
    
Antes de você poder configurar representação, você precisa:
  
- Credenciais administrativas para o Exchange server.
    
- Credenciais de administrador de domínio ou outras credenciais com a permissão para criar e atribuir funções e escopos.
    
- Ferramentas de gerenciamento do Exchange. Eles são instalados no computador do qual você executará os comandos.
    
### <a name="to-configure-impersonation-for-all-users-in-an-organization"></a>Para configurar a representação para todos os usuários em uma organização

1. Abra o Shell de gerenciamento do Exchange. No menu Iniciar, escolha **Todos os programas** > **Microsoft Exchange Server 2013**. 
    
2. Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão de representação ao usuário especificado. O exemplo a seguir mostra como configurar a representação para habilitar uma conta de serviço representar todos os outros usuários em uma organização. 
    
   ```powershell
   New-ManagementRoleAssignment -name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount 
   ```

### <a name="to-configure-impersonation-for-specific-users-or-groups-of-users"></a>Para configurar a representação para usuários específicos ou grupos de usuários

1. Abra o Shell de gerenciamento do Exchange. No menu Iniciar, escolha **Todos os programas** > **Microsoft Exchange Server 2013**. 
    
2. Execute o cmdlet **New-ManagementScope** para criar um escopo ao qual a função de representação pode ser atribuída. Se um escopo existente estiver disponível, você poderá ignorar esta etapa. O exemplo a seguir mostra como criar um escopo de gerenciamento de um grupo específico. 
    
   ```powershell
    New-ManagementScope -Name:scopeName -RecipientRestrictionFilter:recipientFilter
   ```

   O parâmetro _RecipientRestrictionFilter_ do cmdlet **New-ManagementScope** define os membros do escopo. Você pode usar as propriedades do objeto de **identidade** para criar o filtro. O exemplo a seguir é um filtro que restringe o resultado para um único usuário com o usuário nome "João". 
    
   ```powershell
   Name -eq "john"
   ```

3. Execute o cmdlet **New-ManagementRoleAssignment** para adicionar a permissão para representar os membros do escopo especificado. O exemplo a seguir mostra como configurar uma conta de serviço para representar todos os usuários em um escopo. 
    
   ```powershell
    New-ManagementRoleAssignment -Name:impersonationAssignmentName -Role:ApplicationImpersonation -User:serviceAccount -CustomRecipientWriteScope:scopeName
    
   ```


Depois que o administrador concede permissões de representação, você pode usar a conta de serviço para fazer chamadas contra contas de outros usuários. Você pode verificar as atribuições de função usando o cmdlet [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx) . 
  
## <a name="see-also"></a>Confira também

- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
- [Função ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)   
- [New-ManagementRoleAssignment.](http://msdn.microsoft.com/library/34d4f2e3-f2c5-49e1-a6a9-1366da65a78c.aspx)    
- [Get-ManagementRoleAssignment](http://msdn.microsoft.com/library/a3a6ee46-061b-444a-8639-43a416309445.aspx)
    

