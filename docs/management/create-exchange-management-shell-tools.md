---
title: Criar ferramentas do Shell de gerenciamento do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Encontre informações para começar a criação de ferramentas de Shell de gerenciamento do Exchange para o Exchange.
ms.openlocfilehash: e8414460007f333e50c9d596bf977792977b1e4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750958"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="a9d3b-103">Criar ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="a9d3b-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="a9d3b-104">Encontre informações para começar a criação de ferramentas de Shell de gerenciamento do Exchange para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="a9d3b-105">**Aplica-se a:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="a9d3b-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="a9d3b-106">O Shell de gerenciamento do Exchange fornece um conjunto rico de comandos, com base na plataforma do Windows PowerShell para gerenciar o Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="a9d3b-107">Você pode usar os comandos do Shell de gerenciamento do Exchange para automatizar a administração de um servidor executando os comandos de diretamente ou usando scripts de comando.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="a9d3b-108">Se você precisa usar os comandos do Shell de gerenciamento do Exchange dentro de um aplicativo de hospedagem, como um aplicativo administrativo que está executando na área de trabalho do administrador ou por meio de um aplicativo baseado na web, você pode chamar os cmdlets do Shell de gerenciamento do Exchange dentro de seu aplicativo Visual Basic ou c# para gerenciar um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="a9d3b-109">Guia de Introdução com as ferramentas do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="a9d3b-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="a9d3b-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="a9d3b-110"></span></span>

<span data-ttu-id="a9d3b-111">Se você estiver familiarizado com a criação de aplicativos de host do Windows PowerShell e deseja ver um exemplo que mostra como chamar os cmdlets do Shell de gerenciamento do Exchange a partir de um aplicativo ou para ver um exemplo dos tipos de aplicativos que você pode criar usando o Exchange Cmdlets do Shell de gerenciamento, consulte [obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="a9d3b-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="a9d3b-112">Os cmdlets do Shell de gerenciamento do Exchange são extensões do Windows PowerShell, um baseados em tarefa shell de linha de comando e linguagem de script que foi projetada especificamente para administração do sistema.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="a9d3b-113">Windows PowerShell é baseado no .NET Framework e fornece uma API orientado a objetos para o cmdlet, provedor e os desenvolvedores de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="a9d3b-114">Para saber mais sobre programação de Windows PowerShell, consulte o [SDK do Windows PowerShell](http://msdn.microsoft.com/pt-br/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a9d3b-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](http://msdn.microsoft.com/pt-br/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="a9d3b-115">Os cmdlets do Shell de gerenciamento do Exchange aceite e retornam objetos.</span><span class="sxs-lookup"><span data-stu-id="a9d3b-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="a9d3b-116">Para obter uma lista dos cmdlets de shell de gerenciamento do Exchange e seus tipos de entrada e saídos, consulte [cmdlet do Shell de gerenciamento do Exchange de entrada e saída tipos](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="a9d3b-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="a9d3b-117">Nesta se��o</span><span class="sxs-lookup"><span data-stu-id="a9d3b-117">In this section</span></span>

- [<span data-ttu-id="a9d3b-118">Cmdlets do Shell de gerenciamento do Exchange novos e atualizados</span><span class="sxs-lookup"><span data-stu-id="a9d3b-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="a9d3b-119">Entrada de cmdlet do Shell de gerenciamento do Exchange e tipos de saída</span><span class="sxs-lookup"><span data-stu-id="a9d3b-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="a9d3b-120">Obter uma lista de usuários de email usando o Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="a9d3b-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="a9d3b-121">Use a resposta de cmdlet do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="a9d3b-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="a9d3b-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="a9d3b-122">See also</span></span>

- [<span data-ttu-id="a9d3b-123">Namespaces do Shell de gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="a9d3b-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="a9d3b-124">PowerShell do Exchange Server (Shell de gerenciamento do Exchange)</span><span class="sxs-lookup"><span data-stu-id="a9d3b-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/pt-br/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="a9d3b-125">O Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="a9d3b-125">Windows PowerShell</span></span>](http://msdn.microsoft.com/pt-br/library/dd835506%28v=vs.85%29.aspx)
    

