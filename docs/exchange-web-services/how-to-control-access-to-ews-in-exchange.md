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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750696"
---
# <a name="control-access-to-ews-in-exchange"></a>Controlar o acesso a EWS no Exchange

Descubra como controlar o acesso aos EWS para toda a organização, aplicativos ou usuários.
  
Se você estiver usando a API gerenciada de EWS ou EWS diretamente, em seu aplicativo, você pode controlar o acesso a serviços de Web do Exchange (EWS). Se você tiver acesso de administrador para o Exchange server, você pode gerenciar o acesso ao EWS usando o Shell de gerenciamento do Exchange para controlar o acesso globalmente, para cada usuário e para cada aplicativo.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Cmdlets do Shell de gerenciamento do Exchange para configurar o controle de acesso
<a name="bk_Cmdlets"> </a>

Você pode usar os seguintes cmdlets do Shell de gerenciamento do Exchange para exibir a configuração atual do access e definir os controles de acesso do EWS:
  
- [Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - mostra quais parâmetros são definidos para uma caixa de correio específica.   
- [Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - parâmetros de conjuntos para uma caixa de correio específica.    
- [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - mostra os parâmetros para toda a organização.    
- [Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - define os parâmetros para toda a organização. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Exemplos: Controlar o acesso às EWS

Vamos dar uma olhada em alguns cenários que mostram como você pode controlar o acesso ao seu aplicativo.
  
**Tabela 1. Comandos para controlar o acesso às EWS**

|Se você quiser |Use este comando|
|:-----|:-----|
|Impedir que todos os aplicativos cliente usando o EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Isso permite que os aplicativos listados no AllowList para se conectar. Neste exemplo, nenhum aplicativo é incluído no AllowList, para que nenhum aplicativo possa usar o EWS. |
|Uma lista de cliente permitem que aplicativos usam o EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Isso permite que aplicativos específicos para usar o EWS. Neste exemplo, qualquer aplicativo que tenha um agente de usuário a cadeia de caracteres que começa com "OWA /" tem acesso permitido. |
|Permitir que todos os aplicativos de cliente para usar o EWS exceto aqueles especificamente bloqueados. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>Este exemplo bloqueia somente de aplicativos usando o EWS que possuem uma cadeia de caracteres de agente de usuário que inicia com "OWA /". |
|Permitir que todos os aplicativos de cliente para usar o EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Porque nenhuma lista de bloqueios for especificada, todos os aplicativos podem usar EWS. |
|Bloquear toda a organização utilizem EWS. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Permitir que toda a organização usar o EWS. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Bloquear uma caixa de correio individual do usando o EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Permitir que uma caixa de correio individual usar o EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>Confira também

- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)    
- [Controlando o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [O Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

