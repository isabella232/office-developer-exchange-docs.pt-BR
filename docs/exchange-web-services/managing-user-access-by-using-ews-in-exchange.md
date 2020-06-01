---
title: Gerenciando o acesso do usuário usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Descubra quais são as opções de gerenciamento de acesso à conta de usuário para o seu servidor Exchange.
ms.openlocfilehash: 476292d4db206f22cd84134ce2b46957e9fe85fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456238"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="9e1d5-103">Gerenciando o acesso do usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9e1d5-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="9e1d5-104">Descubra quais são as opções de gerenciamento de acesso à conta de usuário para o seu servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="9e1d5-105">Os serviços Web do Exchange (EWS) e a API gerenciada do EWS fornecem um número limitado de operações que você pode usar para gerenciar contas no Exchange Online, o Exchange Online como parte do Office 365 ou uma versão do Exchange a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="9e1d5-106">Você pode usar as operações mostradas na figura a seguir para gerenciar representantes e definir permissões de acesso de pasta para outras contas.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="9e1d5-107">**Operações do EWS para acesso de representante e pasta**</span><span class="sxs-lookup"><span data-stu-id="9e1d5-107">**EWS operations for delegate and folder access**</span></span>

![Opções de gerenciamento de usuário do EWS.](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="9e1d5-109">Se seu aplicativo precisar de controle adicional sobre as contas em um servidor do Exchange, você pode usar os cmdlets do Shell de gerenciamento do Exchange para gerenciar as contas.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-109">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts.</span></span> <span data-ttu-id="9e1d5-110">Você pode chamar os cmdlets do Shell de gerenciamento do Exchange executando um dos seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="9e1d5-110">You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="9e1d5-111">Escrever um aplicativo usando C# ou Visual Basic que chama os cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="9e1d5-112">Você pode examinar o código de exemplo na [documentação da API do Shell de gerenciamento do Exchange](../management/exchange-management-shell.md) para saber como chamar um cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="9e1d5-113">Usando os scripts do Windows PowerShell e do Windows PowerShell para chamar os cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="9e1d5-114">Você pode encontrar uma lista completa do [PowerShell do Exchange Server (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), juntamente com exemplos que mostram como usá-los.</span><span class="sxs-lookup"><span data-stu-id="9e1d5-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="9e1d5-115">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9e1d5-115">See also</span></span>

- [<span data-ttu-id="9e1d5-116">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="9e1d5-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="9e1d5-117">Cmdlets do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9e1d5-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

