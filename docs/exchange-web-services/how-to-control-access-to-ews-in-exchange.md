---
title: Controlar o acesso ao EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Descubra como controlar o acesso ao EWS para usuários, aplicativos ou para toda a organização.
localization_priority: Priority
ms.openlocfilehash: bd65b099ab15c1514945d8a1cfa4e9b1428a4755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456875"
---
# <a name="control-access-to-ews-in-exchange"></a>Controlar o acesso ao EWS no Exchange

Descubra como controlar o acesso ao EWS para usuários, aplicativos ou para toda a organização.
  
Se você estiver usando a API gerenciada do EWS ou o EWS diretamente, em seu aplicativo, você pode controlar o acesso aos serviços Web do Exchange (EWS). Se tiver acesso de administrador ao seu servidor Exchange, você poderá gerenciar o acesso ao EWS usando o Shell de gerenciamento do Exchange para controlar o acesso globalmente, para cada usuário e para cada aplicativo.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Cmdlets do Shell de gerenciamento do Exchange para configurar o controle de acesso
<a name="bk_Cmdlets"> </a>

Você pode usar os seguintes cmdlets do Shell de gerenciamento do Exchange para exibir a configuração atual do Access e definir os controles de acesso do EWS:
  
- [Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) -mostra quais parâmetros estão definidos para uma caixa de correio específica.   
- [Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) -define parâmetros para uma caixa de correio específica.    
- [Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) -mostra os parâmetros para toda a organização.    
- [Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) -define os parâmetros de toda a organização. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Exemplos: controle de acesso ao EWS

Vamos dar uma olhada em alguns cenários que mostram como você pode controlar o acesso ao seu aplicativo.
  
**Tabela 1. Comandos para controlar o acesso ao EWS**

|Se você desejar |Use este comando|
|:-----|:-----|
|Bloquear o uso de todos os aplicativos cliente do EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Isso permite que os aplicativos listados na lista de permissões para se conectar. Neste exemplo, nenhum aplicativo está incluído no Allowlist, portanto, nenhum aplicativo pode usar o EWS. |
|Permite que uma lista de aplicativos cliente use EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Isso permite que aplicativos específicos usem EWS. Neste exemplo, qualquer aplicativo que tenha uma cadeia de caracteres de agente de usuário que comece com "OWA/" tem permissão de acesso. |
|Permitir que todos os aplicativos cliente usem EWS, exceto aqueles especificamente bloqueados. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>Este exemplo apenas impede que aplicativos usem EWS que têm uma cadeia de caracteres de agente de usuário que começa com "OWA/". |
|Permitir que todos os aplicativos cliente usem o EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Como nenhuma blocklist é especificada, todos os aplicativos podem usar o EWS. |
|Bloquear a organização inteira usando o EWS. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Permita que toda a organização Use o EWS. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Bloquear uma caixa de correio individual usando o EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Permitir que uma caixa de correio individual use EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>Confira também

- [Configurando o aplicativo EWS](setting-up-your-ews-application.md)    
- [Controlando o acesso do aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

