---
title: APIs do Office 365 REST para emails, calendários e contatos
manager: sethgros
ms.date: 4/29/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Encontre informações sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.
ms.openlocfilehash: d42d3ff0b68dfbf23d5a4eebb826a6d39a4ac116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750943"
---
# <a name="office-365-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="913c8-103">APIs do Office 365 REST para emails, calendários e contatos</span><span class="sxs-lookup"><span data-stu-id="913c8-103">Office 365 REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="913c8-104">Encontre informações sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="913c8-104">Find information about the Office 365 APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>
  
<span data-ttu-id="913c8-105">O Office 365 e o Exchange Online fornecem uma nova maneira de trabalhar com email, calendários e contatos.</span><span class="sxs-lookup"><span data-stu-id="913c8-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="913c8-106">O email, calendário e APIs REST de contato fornecem uma maneira poderosa e fácil de usar para acessar e manipular dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="913c8-106">The Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="913c8-107">Essas APIs são baseadas em padrões abertos: OAuth versão 2.0 para autenticação e OData versão 4.0 e JSON abstração de dados.</span><span class="sxs-lookup"><span data-stu-id="913c8-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="913c8-108">Isso oferece as seguintes vantagens:</span><span class="sxs-lookup"><span data-stu-id="913c8-108">This provides the following advantages:</span></span>
  
- <span data-ttu-id="913c8-109">Como essas APIs exigem OAuth para autenticação, seu aplicativo não tem que manipular ou armazenar credenciais de usuário.</span><span class="sxs-lookup"><span data-stu-id="913c8-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>
    
- <span data-ttu-id="913c8-110">OAuth torna possível solicitar permissões rigorosamente com escopo para dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="913c8-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="913c8-111">Por exemplo, você pode projetar seu aplicativo para solicitação de permissão e ler apenas o calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="913c8-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>
    
## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="913c8-112">Trabalhar com pastas de email e mala</span><span class="sxs-lookup"><span data-stu-id="913c8-112">Work with email and mail folders</span></span>

<span data-ttu-id="913c8-113">Você pode usar a [API de E-mail](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar, excluir, mover, copiar e enviar email.</span><span class="sxs-lookup"><span data-stu-id="913c8-113">You can use the [Mail API](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="913c8-114">Você também pode obter, criar, atualizar e excluir pastas de email.</span><span class="sxs-lookup"><span data-stu-id="913c8-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="913c8-115">Trabalhar com grupos de calendário, calendários e eventos</span><span class="sxs-lookup"><span data-stu-id="913c8-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="913c8-116">Você pode usar a [API de calendário](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar e excluir eventos.</span><span class="sxs-lookup"><span data-stu-id="913c8-116">You can use the [Calendar API](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx) to get, create, update, and delete events.</span></span> <span data-ttu-id="913c8-117">Você também pode obter, criar, atualizar e excluir grupos de calendário e calendários.</span><span class="sxs-lookup"><span data-stu-id="913c8-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="913c8-118">Trabalhe com contatos e pastas de contatos</span><span class="sxs-lookup"><span data-stu-id="913c8-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="913c8-119">Você pode usar a [API de contatos](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) para obter, criar, atualizar e excluir contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="913c8-119">You can use the [Contacts API](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="913c8-120">Você também pode obter pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="913c8-120">You can also get contact folders.</span></span> 
  
## <a name="work-with-file-providers"></a><span data-ttu-id="913c8-121">Trabalhar com provedores de arquivo</span><span class="sxs-lookup"><span data-stu-id="913c8-121">Work with file providers</span></span>

<span data-ttu-id="913c8-122">Você pode usar a [API REST do arquivo provedores](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) para obter, criar, atualizar e excluir informações sobre provedores de arquivos suportados, como caixa de correio, pasta de recados e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="913c8-122">You can use the [File Providers REST API](http://msdn.microsoft.com/library/8bab5403-de68-4b49-ab19-9a6470f2a2ce%28Office.15%29.aspx) to get, create, update, and delete information about supported file providers, such as mailbox, Dropbox, and so on.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="913c8-123">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="913c8-123">Next steps</span></span>

<span data-ttu-id="913c8-124">Vá direto para a página de [desenvolvimento na plataforma do Office 365](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) para obter mais informações sobre o email, calendário e APIs de contatos, incluindo diretrizes para configurar o seu ambiente e o guia de Introdução com as APIs.</span><span class="sxs-lookup"><span data-stu-id="913c8-124">Head over to the [Developing on the Office 365 platform](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> <span data-ttu-id="913c8-125">Certifique-se também fazer check-out de [projetos de início e códigos de exemplo](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) para ver essas APIs em ação.</span><span class="sxs-lookup"><span data-stu-id="913c8-125">Also be sure to check out the [starter projects and code samples](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="913c8-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="913c8-126">See also</span></span>


- [<span data-ttu-id="913c8-127">Como desenvolver na plataforma do Office 365</span><span class="sxs-lookup"><span data-stu-id="913c8-127">Developing on the Office 365 platform</span></span>](http://msdn.microsoft.com/office/office365/howto/platform-development-overview%28Office.15%29.aspx)
    
- [<span data-ttu-id="913c8-128">Como criar um aplicativo ASP.NET MVC no Office 365</span><span class="sxs-lookup"><span data-stu-id="913c8-128">Building an Office 365 ASP.NET MVC app</span></span>](http://msdn.microsoft.com/office/office365/howto/Build-your-first-ASPNET-MVC-app%28Office.15%29.aspx)
    
- [<span data-ttu-id="913c8-129">Operações REST de email</span><span class="sxs-lookup"><span data-stu-id="913c8-129">Mail REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/mail-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="913c8-130">Operações REST do calendário</span><span class="sxs-lookup"><span data-stu-id="913c8-130">Calendar REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/calendar-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="913c8-131">Operações REST de contatos</span><span class="sxs-lookup"><span data-stu-id="913c8-131">Contacts REST operations</span></span>](http://msdn.microsoft.com/office/office365/api/contacts-rest-operations%28Office.15%29.aspx)
    
- [<span data-ttu-id="913c8-132">Exemplos de código e projetos iniciais de APIs do Office 365</span><span class="sxs-lookup"><span data-stu-id="913c8-132">Office 365 APIs starter projects and code samples</span></span>](http://msdn.microsoft.com/office/office365/howto/Starter-projects-and-code-samples%28Office.15%29.aspx)
    

