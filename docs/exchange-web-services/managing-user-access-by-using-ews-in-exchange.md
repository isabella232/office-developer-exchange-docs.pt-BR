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
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="e8fb9-103">Gerenciando o acesso de usuário usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e8fb9-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="e8fb9-104">Descubra quais são as opções de gerenciamento de acesso da conta de usuário ao seu servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="e8fb9-105">API gerenciada de serviços Web do Exchange (EWS) e o EWS fornecem um número limitado de operações que você pode usar para gerenciar contas no Exchange Online, Exchange Online como parte do Office 365 ou uma versão do Exchange, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="e8fb9-106">Você pode usar as operações mostradas na figura a seguir para gerenciar representantes e definir permissões de acesso de pasta para as outras contas.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="e8fb9-107">**Operações do EWS para acesso de representante e pasta**</span><span class="sxs-lookup"><span data-stu-id="e8fb9-107">**EWS operations for delegate and folder access**</span></span>

![Opções de gerenciamento de usuário do EWS.](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="e8fb9-109">Se seu aplicativo precisa controle adicional sobre as contas em um servidor Exchange, você pode usar os cmdlets do Shell de gerenciamento do Exchange para gerenciar as contas.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-109">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts.</span></span> <span data-ttu-id="e8fb9-110">Você pode chamar os cmdlets do Shell de gerenciamento do Exchange, seguindo um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="e8fb9-110">You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="e8fb9-111">Escrever um aplicativo usando c# ou Visual Basic que chama os cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="e8fb9-112">Você pode examinar o código de exemplo na [documentação de API de Shell de gerenciamento do Exchange](../management/exchange-management-shell.md) para saber como chamar um cmdlet.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="e8fb9-113">Usando o Windows PowerShell e scripts do Windows PowerShell para chamar os cmdlets do Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="e8fb9-114">Você pode encontrar uma lista completa do [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), juntamente com exemplos que mostram como usá-los.</span><span class="sxs-lookup"><span data-stu-id="e8fb9-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="e8fb9-115">Confira também</span><span class="sxs-lookup"><span data-stu-id="e8fb9-115">See also</span></span>

- [<span data-ttu-id="e8fb9-116">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="e8fb9-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="e8fb9-117">Cmdlets do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e8fb9-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

