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
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Controlando o acesso do aplicativo cliente ao EWS no Exchange

Saiba mais sobre as opções para gerenciar o acesso de aplicativos cliente ao EWS.
  
Qualquer aplicativo cliente do EWS que você criar deve ter acesso ao Exchange Online, ao Exchange Online como parte do Office 365, ou a versão do Exchange a partir do Exchange 2013, antes de poder chamar as operações do EWS. Os administradores do servidor de teste ou de produção podem usar o Shell de gerenciamento do Exchange para limitar o acesso ao EWS para todos os usuários e aplicativos, para usuários individuais ou para aplicativos individuais. O controle de acesso para EWS é baseado em contas de domínio. Quando uma conexão é feita com credenciais autenticadas pela autoridade de segurança local, o servidor retorna um erro que indica que somente as contas de domínio podem se conectar. 
  
## <a name="access-control-for-ews-clients-and-users"></a>Controle de acesso para clientes e usuários do EWS
<a name="bk_configure"> </a>

Seu administrador de teste ou de servidor de produção pode configurar o controle de acesso para clientes que se conectam ao EWS das seguintes maneiras: 
  
- Bloqueando a conexão de todos os aplicativos cliente.
    
- Permitindo que aplicativos clientes específicos apenas se conectem.
    
- Permitindo que qualquer aplicativo cliente se conecte, exceto aqueles especificamente bloqueados.
    
- Permitindo que qualquer aplicativo cliente se conecte.
    
Os aplicativos são identificados pela cadeia de caracteres do agente de usuário que eles enviam na solicitação HTTP Web.
  
> [!IMPORTANT]
> O bloqueio no nível do aplicativo não é um recurso de segurança. A cadeia de caracteres do agente do usuário é facilmente falsificada. Se um aplicativo tiver acesso ao EWS, o aplicativo ainda deverá apresentar as credenciais que o servidor autentica para que o aplicativo possa se conectar ao EWS. 
  
Os administradores também podem configurar o controle de acesso para proprietários de caixa de correio que se conectam ao EWS das seguintes maneiras: 
  
- Bloqueando ou permitindo uma organização inteira.
    
- Bloqueando ou permitindo um grupo de usuários identificado por um escopo de autenticação baseada em função que inclui ou exclui proprietários de caixa de correio que não têm acesso ao EWS.
    
- Bloqueando ou permitindo um proprietário de caixa de correio individual.
    
As configurações de controle de acesso específicas substituem as configurações de controle de acesso gerais. Por exemplo, se uma organização negar acesso ao EWS, mas um proprietário de caixa de correio individual tiver permissão de acesso de aplicativo, a configuração individual prevalecerá e o acesso será permitido. 
  
## <a name="delegation-and-ews-access-management"></a>Gerenciamento de delegação e acesso de EWS
<a name="bk_delegation"> </a>

Quando os usuários delegados que não têm acesso ao EWS usam seu aplicativo cliente, eles não poderão acessar a caixa de correio do usuário principal usando o EWS, mesmo que o usuário principal tenha acesso EWS. Se o usuário delegado tiver acesso EWS, o representante será capaz de usar seu aplicativo cliente do EWS para acessar a caixa de correio do usuário principal, mesmo que o usuário principal não tenha acesso EWS. 
  
## <a name="impersonation-and-ews-access-management"></a>Gerenciamento de acesso e representação do EWS
<a name="bk_impersonation"> </a>

Os aplicativos cliente que se conectam ao EWS em nome dos proprietários da caixa de correio podem não conseguir usar as configurações do EWS do proprietário da caixa de correio. Por exemplo, um aplicativo que arquiva mensagens de email de uma empresa deve se conectar ao EWS independentemente das configurações de caixa de correio dos usuários. Outros aplicativos, como clientes de email, precisam usar as configurações do EWS do proprietário da caixa de correio. 
  
Os administradores devem criar uma conta de representação para cada aplicativo ou classe de aplicativo que eles usam no servidor. Isso permitirá que o administrador configure o escopo de controle de acesso baseado em função para todos os usuários que não têm permissões de EWS. 
  
Para habilitar as contas de representação, seu administrador de teste ou de servidor de produção deve executar uma das seguintes ações: 
  
- Adicione o grupo usuários autenticados ao grupo acesso compatível com o anterior ao Win2K. 
    
- Adicione o grupo Exchange Servers ao grupo de acesso de autorização do Windows. 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>Cmdlets do Shell de gerenciamento do Exchange para gerenciamento de acesso
<a name="bk_cmdlets"> </a>

Os administradores usam os seguintes cmdlets do Shell de gerenciamento do Exchange para configurar os controles de acesso do EWS: 
  
- [Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx)   
- [Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx)   
- [Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx)   
- [Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx)
    
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)  
- [Controlar o acesso ao EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)
- [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

