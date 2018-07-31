---
title: API do Microsoft Graph Outlook para emails, calendários e contatos
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Encontre informações sobre a API do Microsoft Graph que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.
ms.openlocfilehash: 3065de389157345afd5ed07e302ace99e2048bdf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353291"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="ff178-103">APIs do Microsoft Graph REST para emails, calendários e contatos</span><span class="sxs-lookup"><span data-stu-id="ff178-103">Microsoft Graph REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="ff178-104">Encontre informações sobre as APIs do Microsoft Graph que você pode usar para acessar email, calendários e contatos no Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ff178-104">Find information about the Microsoft Graph APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>

<span data-ttu-id="ff178-105">O Office 365 e o Exchange Online fornecem uma nova maneira de trabalhar com email, calendários e contatos.</span><span class="sxs-lookup"><span data-stu-id="ff178-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="ff178-106">O Microsoft Graph email, calendário e APIs REST de contato fornecem uma maneira poderosa e fácil de usar para acessar e manipular dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff178-106">The Microsoft Graph Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="ff178-107">Essas APIs são baseadas em padrões abertos: OAuth versão 2.0 para autenticação e OData versão 4.0 e JSON abstração de dados.</span><span class="sxs-lookup"><span data-stu-id="ff178-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="ff178-108">Isso oferece as seguintes vantagens:</span><span class="sxs-lookup"><span data-stu-id="ff178-108">This provides the following advantages:</span></span>

- <span data-ttu-id="ff178-109">Como essas APIs exigem OAuth para autenticação, seu aplicativo não tem que manipular ou armazenar credenciais de usuário.</span><span class="sxs-lookup"><span data-stu-id="ff178-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="ff178-110">OAuth torna possível solicitar permissões rigorosamente com escopo para dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff178-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="ff178-111">Por exemplo, você pode projetar seu aplicativo para solicitação de permissão e ler apenas o calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff178-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="ff178-112">Trabalhar com pastas de email e mala</span><span class="sxs-lookup"><span data-stu-id="ff178-112">Work with email and mail folders</span></span>

<span data-ttu-id="ff178-113">Você pode usar a [API de E-mail](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) para obter, criar, atualizar, excluir, mover, copiar e enviar email.</span><span class="sxs-lookup"><span data-stu-id="ff178-113">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="ff178-114">Você também pode obter, criar, atualizar e excluir pastas de email.</span><span class="sxs-lookup"><span data-stu-id="ff178-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="ff178-115">Trabalhar com grupos de calendário, calendários e eventos</span><span class="sxs-lookup"><span data-stu-id="ff178-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="ff178-116">Você pode usar a [API de calendário](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) para obter, criar, atualizar e excluir eventos.</span><span class="sxs-lookup"><span data-stu-id="ff178-116">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events.</span></span> <span data-ttu-id="ff178-117">Você também pode obter, criar, atualizar e excluir grupos de calendário e calendários.</span><span class="sxs-lookup"><span data-stu-id="ff178-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="ff178-118">Trabalhe com contatos e pastas de contatos</span><span class="sxs-lookup"><span data-stu-id="ff178-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="ff178-119">Você pode usar a [API de contatos](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) para obter, criar, atualizar e excluir contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff178-119">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="ff178-120">Você também pode obter pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="ff178-120">You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="ff178-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ff178-121">Next steps</span></span>

<span data-ttu-id="ff178-122">Vá direto para a página de [documentação do Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) para obter mais informações sobre o email, calendário e APIs de contatos, incluindo diretrizes para configurar o seu ambiente e o guia de Introdução com as APIs.</span><span class="sxs-lookup"><span data-stu-id="ff178-122">Head over to the [Microsoft Graph documentation](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="ff178-123">Certifique-se também fazer check-out do [início rápido](https://developer.microsoft.com/graph/quick-start) e [amostras de código](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) para ver essas APIs em ação.</span><span class="sxs-lookup"><span data-stu-id="ff178-123">Also be sure to check out the [quick starts](https://developer.microsoft.com/graph/quick-start) and [code samples](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ff178-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff178-124">See also</span></span>

- [<span data-ttu-id="ff178-125">Documentação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ff178-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   

