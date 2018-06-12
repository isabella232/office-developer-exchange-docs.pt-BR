---
title: Gerenciando o acesso de usuário usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Descubra quais são as opções de gerenciamento de acesso da conta de usuário ao seu servidor Exchange.
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750857"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Gerenciando o acesso de usuário usando o EWS no Exchange

Descubra quais são as opções de gerenciamento de acesso da conta de usuário ao seu servidor Exchange.
  
API gerenciada de serviços Web do Exchange (EWS) e o EWS fornecem um número limitado de operações que você pode usar para gerenciar contas no Exchange Online, Exchange Online como parte do Office 365 ou uma versão do Exchange, começando com o Exchange 2013. Você pode usar as operações mostradas na figura a seguir para gerenciar representantes e definir permissões de acesso de pasta para as outras contas. 
  
**Operações do EWS para acesso de representante e pasta**

![Opções de gerenciamento de usuário do EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Se seu aplicativo precisa controle adicional sobre as contas em um servidor Exchange, você pode usar os cmdlets do Shell de gerenciamento do Exchange para gerenciar as contas. Você pode chamar os cmdlets do Shell de gerenciamento do Exchange, seguindo um destes procedimentos:
  
- Escrever um aplicativo usando c# ou Visual Basic que chama os cmdlets do Shell de gerenciamento do Exchange. Você pode examinar o código de exemplo na [documentação de API de Shell de gerenciamento do Exchange](../management/exchange-management-shell.md) para saber como chamar um cmdlet. 
    
- Usando o Windows PowerShell e scripts do Windows PowerShell para chamar os cmdlets do Shell de gerenciamento do Exchange. Você pode encontrar uma lista completa do [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), juntamente com exemplos que mostram como usá-los. 
    
## <a name="see-also"></a>Confira também

- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)   
- [Cmdlets do Exchange 2013](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

