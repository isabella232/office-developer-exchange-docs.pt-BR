---
title: Gerenciando o acesso do usuário usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Descubra quais são suas opções para gerenciar o acesso à conta de usuário ao seu Exchange servidor.
ms.openlocfilehash: 431f61a0cbdfcc522eb1481399ffab1f31df9e62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520973"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Gerenciando o acesso do usuário usando o EWS no Exchange

Descubra quais são suas opções para gerenciar o acesso à conta de usuário ao seu Exchange servidor.
  
Exchange Os Serviços Web (EWS) e a API gerenciada do EWS fornecem um número limitado de operações que você pode usar para gerenciar contas no Exchange Online, Exchange Online como parte do Office 365 ou uma versão do Exchange a partir do Exchange 2013. Você pode usar as operações mostradas na figura a seguir para gerenciar representantes e definir permissões de acesso de pasta para outras contas. 
  
**Operações EWS para acesso de representante e pasta**

![Opções de gerenciamento de usuário do EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Se o aplicativo precisar de controle adicional sobre as contas em um servidor Exchange, você poderá usar os cmdlets do Shell de Gerenciamento Exchange gerenciamento para gerenciar as contas. Você pode chamar os cmdlets Exchange Shell de Gerenciamento fazendo um dos seguintes:
  
- Escrevendo um aplicativo usando C# ou Visual Basic que chama os cmdlets Exchange Shell de Gerenciamento. Você pode ver o código de exemplo na documentação [Exchange API](../management/exchange-management-shell.md) do Shell de Gerenciamento para saber como chamar um cmdlet. 
    
- Usando Windows PowerShell e Windows PowerShell para chamar Exchange cmdlets do Shell de Gerenciamento. Você pode encontrar uma lista completa do [Exchange Server PowerShell (Exchange Shell](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)de Gerenciamento) , juntamente com exemplos que mostram como usá-los. 
    
## <a name="see-also"></a>Confira também

- [Como configurar o aplicativo EWS](setting-up-your-ews-application.md)   
- [Exchange Cmdlets 2013](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

