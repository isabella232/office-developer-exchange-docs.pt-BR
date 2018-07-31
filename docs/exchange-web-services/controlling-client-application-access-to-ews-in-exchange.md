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
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Controlando o acesso do aplicativo de cliente para o EWS no Exchange

Saiba mais sobre as opções para gerenciar o acesso do aplicativo cliente para o EWS.
  
Qualquer aplicativo de cliente do EWS que você criar deve ter acesso concedido ao Exchange Online, Exchange Online como parte do Office 365 ou a versão do Exchange começando com o Exchange 2013 antes que ele possa chamar operações do EWS. Administradores de servidor de teste ou de produção podem usar o Shell de gerenciamento do Exchange para limitar o acesso aos EWS para todos os usuários e aplicativos, para usuários individuais ou para aplicativos individuais. Controle de acesso para o EWS baseia-se em contas de domínio. Quando uma conexão é feita com credenciais que são autenticadas pela autoridade de segurança local, o servidor retornará um erro que indica que somente contas de domínio podem se conectar. 
  
## <a name="access-control-for-ews-clients-and-users"></a>Controle de acesso para clientes do EWS e usuários
<a name="bk_configure"> </a>

O administrador do servidor de teste ou de produção pode configurar o controle de acesso para clientes que se conectam ao EWS das seguintes maneiras: 
  
- Impedindo que todos os aplicativos de cliente de se conectar.
    
- Permitindo o cliente específico aplicativos apenas para se conectar.
    
- Permitindo a qualquer aplicativo cliente para se conectar, exceto aqueles especificamente bloqueados.
    
- Permitindo a qualquer aplicativo cliente para se conectar.
    
Aplicativos são identificados pela cadeia de caracteres de agente de usuário que enviam na solicitação HTTP web.
  
> [!IMPORTANT]
> Bloqueio de nível de aplicativo não é um recurso de segurança. A cadeia de caracteres de agente do usuário é falsificada facilmente. Se um aplicativo tem acesso permitido ao EWS, o aplicativo deve ainda apresentar credenciais que o servidor autenticar antes que o aplicativo pode se conectar ao EWS. 
  
Os administradores também podem configurar o controle de acesso para proprietários de caixa de correio que se conectam ao EWS das seguintes maneiras: 
  
- Bloqueando ou permitindo que uma organização inteira.
    
- Bloqueando ou permitindo que um grupo de usuários identificado por um escopo de autenticação baseada em função que inclui ou exclui os proprietários de caixa de correio que não têm acesso ao EWS.
    
- Bloqueando ou permitindo que um proprietário de caixa de correio individuais.
    
Configurações de controle de acesso específicos substituem configurações de controle de acesso geral. Por exemplo, se uma organização negue acesso EWS, mas um proprietário de caixa de correio individual tem permissão de acesso de aplicativo, a configuração individual prevalecerá e acesso é permitido. 
  
## <a name="delegation-and-ews-access-management"></a>Gerenciamento de acesso do EWS e delegação
<a name="bk_delegation"> </a>

Quando o representante de usuários que não têm acesso ao EWS usar seu aplicativo de cliente, eles não poderão acessar a caixa de correio do usuário principal usando EWS, mesmo se o usuário principal tem EWS acessar. Se o usuário delegado tem acesso EWS, o representante será capaz de usar seu aplicativo de cliente do EWS para acessar a caixa de correio do usuário principal, mesmo se o usuário principal EWS não tem acesso. 
  
## <a name="impersonation-and-ews-access-management"></a>Representação e gerenciamento de acesso EWS
<a name="bk_impersonation"> </a>

Aplicativos cliente que se conectam ao EWS em nome de proprietários de caixa de correio podem não ser capazes de usar as configurações do EWS do proprietário da caixa de correio. Por exemplo, um aplicativo que arquiva mensagens são para uma empresa tem para se conectar ao EWS independentemente das configurações de que a caixa de correio dos usuários de email. Outros aplicativos, como clientes de email, é necessário usar as configurações do EWS do proprietário da caixa de correio. 
  
Os administradores devem criar uma conta de representação para cada aplicativo ou classe de aplicativos que eles usam no seu servidor. Isso permitirá que o administrador configure o escopo de controle de acesso baseado em função para todos os usuários que não possui permissões de EWS. 
  
Para habilitar contas de representação, o administrador do servidor de teste ou de produção deve siga um destes procedimentos: 
  
- Adicione o grupo de usuários autenticados ao grupo acesso compatível pré-Win2K. 
    
- Adicione o grupo de servidores do Exchange ao grupo de acesso de autorização do Windows. 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>Cmdlets do Shell de gerenciamento do Exchange para o gerenciamento de acesso
<a name="bk_cmdlets"> </a>

Os administradores usar os seguintes cmdlets do Shell de gerenciamento do Exchange para configurar os controles de acesso do EWS: 
  
- [Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx)   
- [Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx)   
- [Get-OrganizationConfig.](http://technet.microsoft.com/en-us/library/aa997571.aspx)   
- [Set-OrganizationConfig.](http://technet.microsoft.com/en-us/library/aa997443.aspx)
    
## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)  
- [Controlar o acesso a EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)
- [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

