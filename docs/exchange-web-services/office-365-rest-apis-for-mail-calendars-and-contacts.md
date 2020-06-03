---
title: API do Outlook do Microsoft Graph para emails, calendários e contatos
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Encontre informações sobre a API do Microsoft Graph que você pode usar para acessar email, calendários e contatos no Office 365 ou no Exchange Online.
localization_priority: Priority
ms.openlocfilehash: 7ca77596afb59ffab76001abd495de7328d2dd29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463864"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="a241c-103">APIs REST do Microsoft Graph para email, calendários e contatos</span><span class="sxs-lookup"><span data-stu-id="a241c-103">Microsoft Graph REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="a241c-104">Encontre informações sobre as APIs do Microsoft Graph que você pode usar para acessar email, calendários e contatos no Office 365, no Exchange Online ou no Exchange Server em implantações híbridas.</span><span class="sxs-lookup"><span data-stu-id="a241c-104">Find information about the Microsoft Graph APIs that you can use to access mail, calendars, and contacts in Office 365, Exchange Online, or Exchange Server in hybrid deployments.</span></span>

<span data-ttu-id="a241c-105">O Office 365, o Exchange Online e o Exchange Server em implantações híbridas fornecem uma nova maneira de trabalhar com emails, calendários e contatos.</span><span class="sxs-lookup"><span data-stu-id="a241c-105">Office 365, Exchange Online, and Exchange Server in hybrid deployments provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="a241c-106">As APIs REST de email, calendário e contato do Microsoft Graph fornecem uma maneira poderosa e fácil de usar para acessar e manipular dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a241c-106">The Microsoft Graph Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="a241c-107">Essas APIs são baseadas em padrões abertos: OAuth versão 2,0 para autenticação e OData versão 4,0 e JSON para abstração de dados.</span><span class="sxs-lookup"><span data-stu-id="a241c-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="a241c-108">Isto oferece as seguintes vantagens:</span><span class="sxs-lookup"><span data-stu-id="a241c-108">This provides the following advantages:</span></span>

- <span data-ttu-id="a241c-109">Como essas APIs exigem o OAuth para autenticação, seu aplicativo não precisa lidar ou armazenar credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="a241c-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="a241c-110">O OAuth permite que você solicite permissões de escopo rigorosamente para os dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="a241c-110">OAuth makes it possible to request tightly scoped permissions to user data.</span></span> <span data-ttu-id="a241c-111">Por exemplo, você pode criar seu aplicativo para solicitar permissão e ler apenas o calendário de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a241c-111">For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="a241c-112">Trabalhar com email e pastas de email</span><span class="sxs-lookup"><span data-stu-id="a241c-112">Work with email and mail folders</span></span>

<span data-ttu-id="a241c-113">Você pode usar a [API de email](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) para obter, criar, atualizar, excluir, mover, copiar e enviar emails.</span><span class="sxs-lookup"><span data-stu-id="a241c-113">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email.</span></span> <span data-ttu-id="a241c-114">Você também pode obter, criar, atualizar e excluir pastas de email.</span><span class="sxs-lookup"><span data-stu-id="a241c-114">You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="a241c-115">Trabalhar com eventos, calendários e grupos de calendários</span><span class="sxs-lookup"><span data-stu-id="a241c-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="a241c-116">Você pode usar a [API de calendário](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) para obter, criar, atualizar e excluir eventos.</span><span class="sxs-lookup"><span data-stu-id="a241c-116">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events.</span></span> <span data-ttu-id="a241c-117">Você também pode obter, criar, atualizar e excluir grupos de calendários e calendários.</span><span class="sxs-lookup"><span data-stu-id="a241c-117">You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="a241c-118">Trabalhar com contatos e pastas de contatos</span><span class="sxs-lookup"><span data-stu-id="a241c-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="a241c-119">Você pode usar a [API de contatos](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) para obter, criar, atualizar e excluir contatos na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a241c-119">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox.</span></span> <span data-ttu-id="a241c-120">Você também pode obter pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="a241c-120">You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="a241c-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a241c-121">Next steps</span></span>

<span data-ttu-id="a241c-122">Vá para a página [documentação do Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/overview) para obter mais informações sobre as APIs de email, calendário e contatos, incluindo orientações para configurar seu ambiente e introdução às APIs.</span><span class="sxs-lookup"><span data-stu-id="a241c-122">Head over to the [Microsoft Graph documentation](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="a241c-123">Verifique também o [início rápido](https://developer.microsoft.com/graph/quick-start) e os [exemplos de código](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) para ver essas APIs em ação.</span><span class="sxs-lookup"><span data-stu-id="a241c-123">Also be sure to check out the [quick starts](https://developer.microsoft.com/graph/quick-start) and [code samples](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph) to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a241c-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="a241c-124">See also</span></span>

- [<span data-ttu-id="a241c-125">Documentação do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a241c-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   
- [<span data-ttu-id="a241c-126">Requisitos locais para a API REST</span><span class="sxs-lookup"><span data-stu-id="a241c-126">On-premises requirements for the REST API</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api)   

