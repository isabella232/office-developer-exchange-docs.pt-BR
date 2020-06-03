---
title: Criar ferramentas do Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Encontre informações para começar a criar ferramentas do Shell de gerenciamento do Exchange para o Exchange.
ms.openlocfilehash: c6e11fa5b55aa514b12f4f52bc9346ac213d3781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463724"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="9b094-103">Criar ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="9b094-104">Encontre informações para começar a criar ferramentas do Shell de gerenciamento do Exchange para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b094-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="9b094-105">**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="9b094-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="9b094-106">O Shell de gerenciamento do Exchange fornece um conjunto avançado de comandos, com base na plataforma Windows PowerShell, para gerenciar o Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="9b094-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="9b094-107">Você pode usar os comandos do Shell de gerenciamento do Exchange para automatizar a administração de um servidor executando diretamente os comandos ou usando scripts de comando.</span><span class="sxs-lookup"><span data-stu-id="9b094-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="9b094-108">Se você precisar usar os comandos do Shell de gerenciamento do Exchange de dentro de um aplicativo de hospedagem, como um aplicativo administrativo que está sendo executado na área de trabalho do administrador ou por meio de um aplicativo baseado na Web, você poderá chamar os cmdlets do Shell de gerenciamento do Exchange a partir do seu aplicativo do Visual Basic ou C# para gerenciar um servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b094-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="9b094-109">Introdução às ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="9b094-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="9b094-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span></span>

<span data-ttu-id="9b094-111">Se você estiver familiarizado com a criação de aplicativos host do Windows PowerShell e quiser ver um exemplo que mostra como chamar os cmdlets do Shell de gerenciamento do Exchange a partir de um aplicativo ou para ver um exemplo dos tipos de aplicativos que você pode criar usando os cmdlets do Shell de gerenciamento do Exchange, consulte [obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="9b094-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="9b094-112">Os cmdlets do Shell de gerenciamento do Exchange são extensões para o Windows PowerShell, um shell de linha de comando baseado em tarefa e uma linguagem de script projetada especificamente para administração do sistema.</span><span class="sxs-lookup"><span data-stu-id="9b094-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="9b094-113">O Windows PowerShell é criado no .NET Framework e fornece uma API orientada a objeto para desenvolvedores, provedores e aplicativos de host.</span><span class="sxs-lookup"><span data-stu-id="9b094-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="9b094-114">Para saber mais sobre a programação do Windows PowerShell, confira o [SDK do Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9b094-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="9b094-115">Os cmdlets do Shell de gerenciamento do Exchange aceitam e retornam objetos.</span><span class="sxs-lookup"><span data-stu-id="9b094-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="9b094-116">Para obter uma lista de cmdlets do Shell de gerenciamento do Exchange e seus tipos de entrada e saída, consulte [tipos de entrada e saída do cmdlet do Shell de gerenciamento do Exchange](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="9b094-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="9b094-117">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="9b094-117">In this section</span></span>

- [<span data-ttu-id="9b094-118">Cmdlets novos e atualizados do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="9b094-119">Tipos de entrada e de saída de cmdlet do Shell de Gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="9b094-120">Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="9b094-121">Usar a resposta do cmdlet do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="9b094-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="9b094-122">See also</span></span>

- [<span data-ttu-id="9b094-123">Namespaces do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="9b094-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="9b094-124">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="9b094-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="9b094-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="9b094-125">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

