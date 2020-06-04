---
title: Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Saiba como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455748"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a><span data-ttu-id="77b00-103">Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-103">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>

<span data-ttu-id="77b00-104">Saiba como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-104">Find out about maintaining the affinity between a group of subscriptions and the Mailbox server.</span></span>
  
<span data-ttu-id="77b00-105">A afinidade é a associação de uma sequência de mensagens de solicitação e resposta a um servidor de caixa de correio específico.</span><span class="sxs-lookup"><span data-stu-id="77b00-105">Affinity is the association of a sequence of request and response messages with a particular Mailbox server.</span></span> <span data-ttu-id="77b00-106">Para a maioria das funcionalidades no Exchange, a afinidade é manipulada pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="77b00-106">For most functionality in Exchange, affinity is handled by the server.</span></span> <span data-ttu-id="77b00-107">No entanto, as notificações são uma exceção.</span><span class="sxs-lookup"><span data-stu-id="77b00-107">Notifications, however, are an exception.</span></span> <span data-ttu-id="77b00-108">O cliente é responsável por manter a afinidade com o servidor de caixa de correio para assinaturas de notificação.</span><span class="sxs-lookup"><span data-stu-id="77b00-108">The client is responsible for maintaining the affinity with the Mailbox server for notification subscriptions.</span></span> <span data-ttu-id="77b00-109">Essa afinidade permite que o balanceador de carga e os servidores de acesso para cliente entre o cliente e o servidor direcionem as assinaturas de notificação e as solicitações relacionadas para o servidor de caixa de correio que mantém a assinatura.</span><span class="sxs-lookup"><span data-stu-id="77b00-109">This affinity enables the load balancer and Client Access servers between the client and the server to route notification subscriptions and related requests to the Mailbox server that maintains the subscription.</span></span> <span data-ttu-id="77b00-110">Sem a afinidade, a solicitação pode ser roteada para um servidor de caixa de correio diferente que não inclua as assinaturas do cliente, o que pode causar o retorno de um erro [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="77b00-110">Without affinity, the request might get routed to a different Mailbox server that does not include the client's subscriptions, which can cause an [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) error to be returned.</span></span> 
  
## <a name="how-is-affinity-maintained"></a><span data-ttu-id="77b00-111">Como a afinidade é mantida?</span><span class="sxs-lookup"><span data-stu-id="77b00-111">How is affinity maintained?</span></span>
<span data-ttu-id="77b00-112"><a name="bk_howmaintained"> </a></span><span class="sxs-lookup"><span data-stu-id="77b00-112"><a name="bk_howmaintained"> </a></span></span>

<span data-ttu-id="77b00-113">A afinidade no Exchange é baseada em cookies.</span><span class="sxs-lookup"><span data-stu-id="77b00-113">Affinity in Exchange is cookie based.</span></span> <span data-ttu-id="77b00-114">O cliente dispara a criação do cookie incluindo cabeçalhos específicos na solicitação de assinatura e, em seguida, a resposta de assinatura contém o cookie.</span><span class="sxs-lookup"><span data-stu-id="77b00-114">The client triggers the creation of the cookie by including specific headers in the subscription request, and then the subscription response contains the cookie.</span></span> <span data-ttu-id="77b00-115">O cliente, em seguida, envia esse cookie em solicitações subsequentes para garantir que a solicitação seja encaminhada para o servidor de caixa de correio certo.</span><span class="sxs-lookup"><span data-stu-id="77b00-115">The client then sends that cookie in subsequent requests to ensure that the request is routed to the right Mailbox server.</span></span>
  
<span data-ttu-id="77b00-116">Mais especificamente, a afinidade no Exchange é manipulada pelo seguinte:</span><span class="sxs-lookup"><span data-stu-id="77b00-116">More specifically, affinity in Exchange is handled by the following:</span></span> 
  
- <span data-ttu-id="77b00-117">X-AnchorMailbox — um cabeçalho HTTP incluído na solicitação de assinatura inicial.</span><span class="sxs-lookup"><span data-stu-id="77b00-117">X-AnchorMailbox — An HTTP header that is included in the initial subscription request.</span></span> <span data-ttu-id="77b00-118">Ele identifica a primeira caixa de correio em um grupo de caixas de correio que compartilham a afinidade com o mesmo servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-118">It identifies the first mailbox in a group of mailboxes that share affinity with the same Mailbox server.</span></span>
    
- <span data-ttu-id="77b00-119">X-PreferServerAffinity — um cabeçalho HTTP que é incluído na solicitação de assinatura inicial com o cabeçalho X-AnchorMailbox e é definido como true para indicar que o cliente está solicitando que a afinidade seja mantida com o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-119">X-PreferServerAffinity — An HTTP header that is included in the initial subscription request with the X-AnchorMailbox header and is set to true to indicate that the client is requesting that affinity be maintained with the Mailbox server.</span></span>
    
- <span data-ttu-id="77b00-120">X-BackEndOverrideCookie — um cookie incluído na resposta inicial da assinatura e contém um cookie que o balanceador de carga e o servidor de acesso para cliente usam para rotear as solicitações subsequentes para o mesmo servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-120">X-BackEndOverrideCookie — A cookie that is included in the initial subscription response and contains a cookie that the load balancer and Client Access server use to route subsequent requests to the same Mailbox server.</span></span>
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a><span data-ttu-id="77b00-121">Como faço para manter a afinidade usando a API gerenciada do EWS ou o EWS?</span><span class="sxs-lookup"><span data-stu-id="77b00-121">How do I maintain affinity by using the EWS Managed API or EWS?</span></span>
<span data-ttu-id="77b00-122"><a name="bk_howdoimaintain"> </a></span><span class="sxs-lookup"><span data-stu-id="77b00-122"><a name="bk_howdoimaintain"> </a></span></span>

<span data-ttu-id="77b00-123">Você pode usar as mesmas etapas para manter a afinidade para várias assinaturas de caixa de correio e seus servidores de caixa de correio, independentemente de você estar usando o streaming, pull ou notificações por push, e independente se você está direcionando um servidor local do Exchange ou o Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="77b00-123">You can use the same steps to maintain affinity for multiple mailbox subscriptions and their Mailbox servers, regardless of whether you are using streaming, pull, or push notifications, and regardless of whether you're targeting an Exchange on-premises server or Exchange Online.</span></span>
  
1. <span data-ttu-id="77b00-124">Para cada caixa de correio, [ligue para descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e obtenha as configurações de usuário do GroupingInformation e do ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="77b00-124">For each mailbox, [call Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and get the GroupingInformation and ExternalEwsUrl user settings.</span></span> <span data-ttu-id="77b00-125">Para descoberta automática SOAP, você usa o elemento [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) e a descoberta automática do Pox, você usa o elemento [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="77b00-125">For SOAP Autodiscover, you use the [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) element, and for POX Autodiscover, you use the [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) element.</span></span> 
    
2. <span data-ttu-id="77b00-126">Usando as configurações do GroupingInformation e do ExternalEwsUrl das respostas da descoberta automática, coloque as caixas de correio com o mesmo valor concatenado ExternalEwsUrl e GroupingInformation no mesmo grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-126">Using the GroupingInformation and ExternalEwsUrl settings from the Autodiscover responses, place mailboxes with the same ExternalEwsUrl and GroupingInformation concatenated value in the same group.</span></span> <span data-ttu-id="77b00-127">Se qualquer grupo tiver mais de 200 caixas de correio, quebre os grupos para baixo, de modo que cada grupo não tenha mais de 200 caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-127">If any groups have more than 200 mailboxes, break the groups down further so that each group has no more than 200 mailboxes.</span></span>
    
3. <span data-ttu-id="77b00-128">Crie e use um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) para o restante do procedimento.</span><span class="sxs-lookup"><span data-stu-id="77b00-128">Create and use one [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) object for the rest of the procedure.</span></span> <span data-ttu-id="77b00-129">Quando você usa o mesmo objeto **ExchangeService** , cookies e cabeçalhos (quando são definidos) são mantidos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="77b00-129">When you use the same **ExchangeService** object, cookies and headers (when they are set) are automatically maintained.</span></span> <span data-ttu-id="77b00-130">Observe que, se você não pretende agrupar assinaturas de streaming em uma única conexão, você tem liberdade para criar um objeto **ExchangeService** diferente para cada usuário representado.</span><span class="sxs-lookup"><span data-stu-id="77b00-130">Note that if you do not intend to group streaming subscriptions into a single connection, you are free to create a different **ExchangeService** object for each impersonated user.</span></span> 
    
4. <span data-ttu-id="77b00-131">[Envie uma](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) solicitação de assinatura para o usuário cujo nome de usuário aparece primeiro quando todos os usuários no grupo são classificados alfabeticamente (faremos referência a esse usuário como o usuário de caixa de correio de ancoragem).</span><span class="sxs-lookup"><span data-stu-id="77b00-131">[Send a subscription](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) request for the user whose user name appears first when all users in the group are sorted alphabetically (we'll refer to this user as the anchor mailbox user).</span></span> <span data-ttu-id="77b00-132">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="77b00-132">Do the following:</span></span> 
    
  - <span data-ttu-id="77b00-133">Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário da caixa de correio de âncora.</span><span class="sxs-lookup"><span data-stu-id="77b00-133">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user.</span></span>
    
  - <span data-ttu-id="77b00-134">Inclua o cabeçalho X-PreferServerAffinity com um valor definido como true.</span><span class="sxs-lookup"><span data-stu-id="77b00-134">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="77b00-135">Use a função [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (o tipo [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="77b00-135">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
5. <span data-ttu-id="77b00-136">Na resposta de assinatura, obtenha o valor X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="77b00-136">In the subscription response, get the X-BackEndOverrideCookie value.</span></span> <span data-ttu-id="77b00-137">Inclua esse valor em cada uma das solicitações de assinatura subsequentes para os usuários desse grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-137">Include this value in each of the subsequent subscription requests for users in this group.</span></span>
    
6. <span data-ttu-id="77b00-138">Para cada usuário adicional no grupo, envie uma solicitação de assinatura e faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="77b00-138">For each additional user in the group, send a subscription request and do the following:</span></span>
    
  - <span data-ttu-id="77b00-139">Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário de caixa de correio de âncora do grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-139">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user for the group.</span></span>
    
  - <span data-ttu-id="77b00-140">Inclua o cabeçalho X-PreferServerAffinity com um valor definido como true.</span><span class="sxs-lookup"><span data-stu-id="77b00-140">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="77b00-141">Inclua o X-BackEndOverrideCookie retornado na resposta de assinatura do usuário da caixa de correio de ancoragem.</span><span class="sxs-lookup"><span data-stu-id="77b00-141">Include the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response.</span></span>
    
  - <span data-ttu-id="77b00-142">Use a função [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (o tipo [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="77b00-142">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
    <span data-ttu-id="77b00-143">Observe que o servidor usa os valores X-PreferServerAffinity e X-BackendOverrideCookie juntos para executar o roteamento para o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-143">Note that the server uses the X-PreferServerAffinity and X-BackendOverrideCookie values together to perform the routing to the mailbox server.</span></span> <span data-ttu-id="77b00-144">O cabeçalho X-AnchorMailbox também é necessário, mas é ignorado pelo servidor se os outros dois valores forem válidos.</span><span class="sxs-lookup"><span data-stu-id="77b00-144">The X-AnchorMailbox header is also required, but is ignored by the server if the other two values are valid.</span></span> <span data-ttu-id="77b00-145">Se X-AnchorMailbox e X-PreferServerAffinity estiverem em uma solicitação e X-BackendOverrideCookie não for incluído, o valor X-AnchorMailbox será usado para encaminhar as solicitações.</span><span class="sxs-lookup"><span data-stu-id="77b00-145">If X-AnchorMailbox and X-PreferServerAffinity are in a request and X-BackendOverrideCookie is not included, the X-AnchorMailbox value is used to route the requests.</span></span>
    
    <span data-ttu-id="77b00-146">Como os valores X-PreferServerAffinity e X-BackendOverrideCookie executam o roteamento, se a caixa de correio de ancoragem for movida para outro grupo ou servidor, a lógica não será alterada porque o X-BackendOverrideCookie encaminhará a solicitação para o servidor correto para o grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-146">Because the X-PreferServerAffinity and X-BackendOverrideCookie values perform the routing, if the anchor mailbox ever moves to another group or server, the logic does not change because the X-BackendOverrideCookie will route the request to the correct server for the group.</span></span>
    
7. <span data-ttu-id="77b00-147">Envie uma única solicitação de [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) para o grupo e faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="77b00-147">Send a single [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) requests for the group, and do the following:</span></span> 
    
  - <span data-ttu-id="77b00-148">Inclua os valores [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) retornados em cada uma das respostas de assinatura individuais para caixas de correio no grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-148">Include the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values returned in each of the individual subscription responses for mailboxes in the group.</span></span> 
    
  - <span data-ttu-id="77b00-149">Se houver mais de 200 assinaturas para o grupo, crie várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="77b00-149">If more than 200 subscriptions exist for the group, create multiple requests.</span></span> <span data-ttu-id="77b00-150">O número máximo de valores de [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) a serem incluídos em uma solicitação é 200.</span><span class="sxs-lookup"><span data-stu-id="77b00-150">The maximum number of [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values to include in a request is 200.</span></span> 
    
  - <span data-ttu-id="77b00-151">Se você precisar de mais conexões do que as disponíveis para a caixa de correio de destino, use a conta de serviço para representar a caixa de correio de ancoragem para o grupo; caso contrário, não use representação.</span><span class="sxs-lookup"><span data-stu-id="77b00-151">If you need more connections than are available to the target mailbox, use the service account to impersonate the anchor mailbox for the group; otherwise, do not use impersonation.</span></span> <span data-ttu-id="77b00-152">O ideal é que você queira representar uma caixa de correio exclusiva por solicitação [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) para que você nunca encontre limites de limitação.</span><span class="sxs-lookup"><span data-stu-id="77b00-152">Ideally, you want to impersonate a unique mailbox per [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) request so that you never encounter throttling limits.</span></span> 
    
  - <span data-ttu-id="77b00-153">Use ApplicationImpersonation se você precisar [de mais conexões do que estão disponíveis para a caixa de correio de destino](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); caso contrário, não use ApplicationImpersonation.</span><span class="sxs-lookup"><span data-stu-id="77b00-153">Use ApplicationImpersonation if you need [more connections than are available to the target mailbox](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); otherwise, do not use ApplicationImpersonation.</span></span>
    
  - <span data-ttu-id="77b00-154">Inclua o cabeçalho X-PreferServerAffinity e defina-o como true.</span><span class="sxs-lookup"><span data-stu-id="77b00-154">Include the X-PreferServerAffinity header and set it to true.</span></span> <span data-ttu-id="77b00-155">Esse valor será incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="77b00-155">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
  - <span data-ttu-id="77b00-156">Inclua o X-BackEndOverrideCookie para o grupo (o X-BackEndOverrideCookie que foi retornado na resposta de assinatura do usuário da caixa de correio de ancoragem).</span><span class="sxs-lookup"><span data-stu-id="77b00-156">Include the X-BackEndOverrideCookie for the group (the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response).</span></span> <span data-ttu-id="77b00-157">Esse valor será incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="77b00-157">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
8. <span data-ttu-id="77b00-158">Passe os eventos retornados para um thread separado para processamento.</span><span class="sxs-lookup"><span data-stu-id="77b00-158">Pass the returned events to a separate thread for processing.</span></span>
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a><span data-ttu-id="77b00-159">Que valores de limitação Eu preciso considerar?</span><span class="sxs-lookup"><span data-stu-id="77b00-159">What throttling values do I need to take into consideration?</span></span>
<span data-ttu-id="77b00-160"><a name="bk_throttling"> </a></span><span class="sxs-lookup"><span data-stu-id="77b00-160"><a name="bk_throttling"> </a></span></span>

<span data-ttu-id="77b00-161">Ao planejar sua implementação de notificação, você deverá levar em consideração dois valores: o número de conexões e o número de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="77b00-161">As you plan your notification implementation, you'll want to take two values into consideration: the number of connections, and the number of subscriptions.</span></span> <span data-ttu-id="77b00-162">A tabela a seguir lista os valores padrão para cada configuração de [limitação](ews-throttling-in-exchange.md) e como as configurações são usadas.</span><span class="sxs-lookup"><span data-stu-id="77b00-162">The following table lists the default values for each [throttling](ews-throttling-in-exchange.md) setting and how the settings are used.</span></span> <span data-ttu-id="77b00-163">Para cada valor, o orçamento é alocado para a caixa de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="77b00-163">For each value, the budget is allocated to the target mailbox.</span></span> <span data-ttu-id="77b00-164">Por esse motivo, usar a representação para obter conexões adicionais é uma etapa obrigatória em muitos cenários.</span><span class="sxs-lookup"><span data-stu-id="77b00-164">For this reason, using impersonation to gain additional connections is a required step in many scenarios.</span></span> 
  
<span data-ttu-id="77b00-165">**Tabela 1. Valores de limitação padrão**</span><span class="sxs-lookup"><span data-stu-id="77b00-165">**Table 1. Default throttling values**</span></span>

|<span data-ttu-id="77b00-166">**Área de consideração**</span><span class="sxs-lookup"><span data-stu-id="77b00-166">**Area of consideration**</span></span>|<span data-ttu-id="77b00-167">**Configuração de limitação**</span><span class="sxs-lookup"><span data-stu-id="77b00-167">**Throttling setting**</span></span>|<span data-ttu-id="77b00-168">**Valor padrão**</span><span class="sxs-lookup"><span data-stu-id="77b00-168">**Default value**</span></span>|<span data-ttu-id="77b00-169">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77b00-169">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="77b00-170">Conexões de streaming</span><span class="sxs-lookup"><span data-stu-id="77b00-170">Streaming connections</span></span>  <br/> |<span data-ttu-id="77b00-171">Limite de conexão deslocada padrão</span><span class="sxs-lookup"><span data-stu-id="77b00-171">Default hanging connection limit</span></span>  <br/> |<span data-ttu-id="77b00-172">10 para o Exchange Online</span><span class="sxs-lookup"><span data-stu-id="77b00-172">10 for Exchange Online</span></span>  <br/> <span data-ttu-id="77b00-173">3 para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77b00-173">3 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="77b00-174">O número máximo de conexões de fluxo simultâneos que uma conta pode ter aberto no servidor de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="77b00-174">The maximum number of concurrent streaming connections that an account can have open on the server at one time.</span></span> <span data-ttu-id="77b00-175">Para trabalhar dentro desse limite, use uma conta de serviço com a função ApplicationImpersonation atribuída às caixas de correio de destino e represente o primeiro usuário em cada grupo de ID de assinatura ao obter eventos em fluxo.</span><span class="sxs-lookup"><span data-stu-id="77b00-175">To work within this limit, use a service account with the ApplicationImpersonation role assigned for the target mailboxes, and impersonate the first user in each subscription ID group when getting streamed events.</span></span>  <br/> |
|<span data-ttu-id="77b00-176">Conexões pull ou push</span><span class="sxs-lookup"><span data-stu-id="77b00-176">Pull or push connections</span></span>  <br/> |<span data-ttu-id="77b00-177">EWSMaxConcurrency</span><span class="sxs-lookup"><span data-stu-id="77b00-177">EWSMaxConcurrency</span></span>  <br/> |<span data-ttu-id="77b00-178">27</span><span class="sxs-lookup"><span data-stu-id="77b00-178">27</span></span>  <br/> |<span data-ttu-id="77b00-179">O número máximo de conexões simultâneas de pull ou push (solicitações que foram recebidas, mas que ainda não responderam a) que uma conta pode ter aberto no servidor ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="77b00-179">The maximum number of concurrent pull or push connections (requests that have been received but not yet responded to) that an account can have open on the server at one time.</span></span>  <br/> |
|<span data-ttu-id="77b00-180">Assinaturas</span><span class="sxs-lookup"><span data-stu-id="77b00-180">Subscriptions</span></span>  <br/> |<span data-ttu-id="77b00-181">EWSMaxSubscriptions</span><span class="sxs-lookup"><span data-stu-id="77b00-181">EWSMaxSubscriptions</span></span>  <br/> |<span data-ttu-id="77b00-182">20 para o Exchange Online</span><span class="sxs-lookup"><span data-stu-id="77b00-182">20 for Exchange Online</span></span>  <br/> <span data-ttu-id="77b00-183">5000 para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="77b00-183">5000 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="77b00-184">O número máximo de assinaturas não expiradas que uma conta pode ter ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="77b00-184">The maximum number of nonexpired subscriptions that an account can have at one time.</span></span> <span data-ttu-id="77b00-185">Esse valor é decrementado quando a assinatura é criada no servidor.</span><span class="sxs-lookup"><span data-stu-id="77b00-185">This value is decremented when the subscription is created on the server.</span></span>  <br/> |
   
<span data-ttu-id="77b00-186">O exemplo a seguir mostra como os orçamentos são tratados entre qualquer caixa de correio de destino e a conta de serviço que tem a função [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) atribuída às caixas de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="77b00-186">The following example shows how budgets are handled between any target mailbox and the service account that has the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role assigned for the target mailboxes.</span></span> 
  
- <span data-ttu-id="77b00-187">ServiceAccount1 (SA1) representa muitos usuários (M1, m2, M3 e assim por diante) e cria assinaturas para cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-187">ServiceAccount1 (sa1) impersonates many users (m1, m2, m3, and so on) and creates subscriptions for each mailbox.</span></span> <span data-ttu-id="77b00-188">Observe que, quando as assinaturas são criadas, o proprietário da assinatura é SA1, portanto, quando SA1 abre uma conexão com as assinaturas, o EWS impõe que as assinaturas sejam de Propriedade do SA1.</span><span class="sxs-lookup"><span data-stu-id="77b00-188">Note that when the subscriptions are created, the subscription owner is sa1, so when sa1 opens a connection with the subscriptions, EWS enforces that the subscriptions are owned by sa1.</span></span>
    
- <span data-ttu-id="77b00-189">O Sa1 pode abrir a conexão das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="77b00-189">Sa1 can open the connection in the following ways:</span></span>
    
1. <span data-ttu-id="77b00-190">Sem representação, portanto, a conexão é cobrada em relação ao SA1.</span><span class="sxs-lookup"><span data-stu-id="77b00-190">Without impersonation, so the connection is charged against sa1.</span></span>
    
2. <span data-ttu-id="77b00-191">Ao representar qualquer um dos usuários — M1, por exemplo, para que a conexão seja cobrada por uma cópia do orçamento do m1's.</span><span class="sxs-lookup"><span data-stu-id="77b00-191">By impersonating any of the users — m1 for example — so that the connection is charged against a copy of m1's budget.</span></span> <span data-ttu-id="77b00-192">(O próprio M1 pode abrir dez conexões usando o Exchange Online e todas as contas de serviço que estão representando M1 podem abrir dez conexões usando o orçamento copiado.)</span><span class="sxs-lookup"><span data-stu-id="77b00-192">(M1 itself can open ten connections by using Exchange Online, and all service accounts impersonating m1 can open ten connections by using the copied budget.)</span></span>
    
- <span data-ttu-id="77b00-193">Se o limite de conexão for atingido, as seguintes soluções alternativas estarão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="77b00-193">If the connection limit is hit, the following workarounds are available:</span></span>
    
  - <span data-ttu-id="77b00-194">Se a opção 1 for usada, o administrador pode criar várias contas de serviço para representar usuários adicionais.</span><span class="sxs-lookup"><span data-stu-id="77b00-194">If option 1 is used, the administrator can create multiple service accounts to impersonate additional users.</span></span>
    
  - <span data-ttu-id="77b00-195">Se a opção 2 for usada, o código pode representar outro usuário, m2, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="77b00-195">If option 2 is used, the code can impersonate another user — m2 for example.</span></span>
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a><span data-ttu-id="77b00-196">Exemplo: manutenção da afinidade entre um grupo de assinaturas e o servidor de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="77b00-196">Example: Maintaining affinity between a group of subscriptions and the Mailbox server</span></span>
<span data-ttu-id="77b00-197"><a name="bk_ce"> </a></span><span class="sxs-lookup"><span data-stu-id="77b00-197"><a name="bk_ce"> </a></span></span>

<span data-ttu-id="77b00-198">Ok, vamos vê-lo em ação.</span><span class="sxs-lookup"><span data-stu-id="77b00-198">Okay, let's see it in action.</span></span> <span data-ttu-id="77b00-199">O exemplo de código a seguir mostra como agrupar usuários e usar os cabeçalhos x-AnchorMailbox e X-PreferServerAffinity e o cookie X-BackendOverrideCookie para manter a afinidade com o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-199">The following code example shows you how to group users and use the X-AnchorMailbox and X-PreferServerAffinity headers and the X-BackendOverrideCookie cookie to maintain affinity with the Mailbox server.</span></span> <span data-ttu-id="77b00-200">Como os cabeçalhos e o cookie são de importância principal na história da afinidade, este exemplo se concentra nas solicitações e respostas XML do EWS.</span><span class="sxs-lookup"><span data-stu-id="77b00-200">Because the headers and the cookie are of primary importance in the affinity story, this example focuses on the EWS XML requests and responses.</span></span> <span data-ttu-id="77b00-201">Para usar a API gerenciada do EWS para criar o corpo das solicitações de assinatura e respostas, consulte [Stream notifications about Mailbox Events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) and [pull notifications about Mailbox Events by using the EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="77b00-201">To use the EWS Managed API to create the body of the subscription requests and responses, see [Stream notifications about mailbox events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) and [Pull notifications about mailbox events by using EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="77b00-202">Esta seção inclui etapas adicionais específicas para manter a afinidade e adicionar os cabeçalhos às suas solicitações.</span><span class="sxs-lookup"><span data-stu-id="77b00-202">This section includes additional steps particular to maintaining affinity and adding the headers to your requests.</span></span>
  
<span data-ttu-id="77b00-203">Este exemplo tem quatro usuários: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com e sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="77b00-203">This example has four users: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com, and sadie@contoso.com.</span></span> <span data-ttu-id="77b00-204">A figura a seguir mostra as configurações de [descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) do GroupingInformation e do ExternalEwsUrl para os usuários.</span><span class="sxs-lookup"><span data-stu-id="77b00-204">The following figure shows the GroupingInformation and ExternalEwsUrl [Autodiscover settings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) for the users.</span></span> 
  
<span data-ttu-id="77b00-205">**Figura 1. Configurações de descoberta automática usadas para agrupar caixas de correio**</span><span class="sxs-lookup"><span data-stu-id="77b00-205">**Figure 1. Autodiscover settings used to group mailboxes**</span></span>

![A table that shows the GroupingInformation and ExternalEwsUrl values for each of the users.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
<span data-ttu-id="77b00-207">Usando as configurações das respostas de descoberta automática, as caixas de correio são agrupadas pelo valor concatenado das configurações GroupingInformation e ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="77b00-207">Using the settings from the Autodiscover responses, the mailboxes are grouped by the concatenated value of the GroupingInformation and ExternalEwsUrl settings.</span></span> <span data-ttu-id="77b00-208">Neste exemplo, Alfred e Sadie têm os mesmos valores, portanto, estão em um grupo, e alisa e Ronnie compartilham os mesmos valores, portanto, estão em outro grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-208">In this example, Alfred and Sadie have the same values, so they are in one group, and Alisa and Ronnie share the same values, so they are in another group.</span></span>
  
<span data-ttu-id="77b00-209">**Figura 2. Criando grupos de caixa de correio**</span><span class="sxs-lookup"><span data-stu-id="77b00-209">**Figure 2. Creating mailbox groups**</span></span>

![A table that shows how mailbox groups are created using Autodiscover settings.](media/Exchange2013_NotificationAffinityGrouping.png)
  
<span data-ttu-id="77b00-211">Para o objetivo deste exemplo, vamos nos concentrar no grupo A. Devemos usar as mesmas etapas para o grupo B, mas usar um valor X-AnchorMailbox diferente para esse grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-211">For the purpose of this example, we'll focus on Group A. We would use the same steps for group B, but use a different X-AnchorMailbox value for that group.</span></span>
  
<span data-ttu-id="77b00-212">Usando o [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), crie a solicitação de assinatura da caixa de correio de âncora (Alfred@contoso.com), com o cabeçalho X-AnchorMailbox definido para o endereço de email e um valor de cabeçalho x-PreferServerAffinity de true.</span><span class="sxs-lookup"><span data-stu-id="77b00-212">Using [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), create the subscription request for the anchor mailbox (alfred@contoso.com), with the X-AnchorMailbox header set to the their email address and an X-PreferServerAffinity header value of true.</span></span> <span data-ttu-id="77b00-213">A definição desses dois valores de cabeçalho disparará o servidor para criar um X-BackEndOverrideCookie para a resposta.</span><span class="sxs-lookup"><span data-stu-id="77b00-213">Setting these two header values will trigger the server to create an X-BackEndOverrideCookie for the response.</span></span>
  
<span data-ttu-id="77b00-214">Se você estiver usando a API gerenciada do EWS, use o método[Add](https://msdn.microsoft.com/library/cy7xta5e) [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)para adicionar os dois cabeçalhos à sua solicitação de assinatura, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="77b00-214">If you're using the EWS Managed API, use the [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](https://msdn.microsoft.com/library/cy7xta5e) method to add the two headers to your subscription request, as shown.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

<span data-ttu-id="77b00-215">Portanto, a solicitação de assinatura do Alfred tem a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="77b00-215">So Alfred's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="77b00-216">A seguinte mensagem XML é a resposta à solicitação de assinatura do Alfred e inclui o X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="77b00-216">The following XML message is the response to Alfred's subscription request, and it includes the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="77b00-217">Reenvie este cookie para todas as solicitações subsequentes para os usuários deste grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-217">Resend this cookie for all subsequent requests for users in this group.</span></span> <span data-ttu-id="77b00-218">Observe que a resposta também contém cookies adicionais, como o cookie exchangecookie usado pelo Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="77b00-218">Notice that the response also contains additional cookies, such as the exchangecookie cookie used by Exchange 2010.</span></span> <span data-ttu-id="77b00-219">Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013, ignore exchangecookie se estiver incluído em solicitações de assinatura subsequentes.</span><span class="sxs-lookup"><span data-stu-id="77b00-219">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013, ignore exchangecookie if it is included in subsequent subscription requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="77b00-220">Usando o X-BackEndOverrideCookie da resposta de Alfred e o cabeçalho X-AnchorMailbox, a solicitação de assinatura é criada para o Sadie, o outro membro da solicitação de assinatura de grupo A. Sadie tem a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="77b00-220">Using the X-BackEndOverrideCookie from Alfred's response and the X-AnchorMailbox header, the subscription request is created for Sadie, the other member of Group A. Sadie's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="77b00-221">A resposta de assinatura do Sadie tem a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="77b00-221">Sadie's subscription response looks like this.</span></span> <span data-ttu-id="77b00-222">Observe que ele não inclui o X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="77b00-222">Note that it does not include the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="77b00-223">O cliente é responsável por armazenar em cache esse valor para solicitações futuras.</span><span class="sxs-lookup"><span data-stu-id="77b00-223">The client is responsible for caching that value for future requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="77b00-224">Usando os valores [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) das respostas de assinatura, uma solicitação de operação [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) foi criada para todas as assinaturas do grupo.</span><span class="sxs-lookup"><span data-stu-id="77b00-224">Using the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values from the subscription responses, a [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) operation request was created for all the subscriptions in the group.</span></span> <span data-ttu-id="77b00-225">Como há menos de 200 assinaturas nesse grupo, todas elas são enviadas em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="77b00-225">Because there are less than 200 subscriptions in this group, they are all sent in one request.</span></span> <span data-ttu-id="77b00-226">O cabeçalho X-PreferServerAffinity é definido como true e o X-BackEndOverrideCookie está incluído.</span><span class="sxs-lookup"><span data-stu-id="77b00-226">The X-PreferServerAffinity header is set to true and the X-BackEndOverrideCookie is included.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="77b00-227">Os eventos retornados são passados para um thread separado para processamento.</span><span class="sxs-lookup"><span data-stu-id="77b00-227">The returned events are then passed to a separate thread for processing.</span></span>
  
## <a name="how-has-affinity-changed"></a><span data-ttu-id="77b00-228">Como a afinidade foi alterada?</span><span class="sxs-lookup"><span data-stu-id="77b00-228">How has affinity changed?</span></span>
<span data-ttu-id="77b00-229"><a name="bk_howchanged"> </a></span><span class="sxs-lookup"><span data-stu-id="77b00-229"><a name="bk_howchanged"> </a></span></span>

<span data-ttu-id="77b00-230">No Exchange 2010, as assinaturas são mantidas no servidor de acesso para cliente, conforme mostrado na Figura 3.</span><span class="sxs-lookup"><span data-stu-id="77b00-230">In Exchange 2010, subscriptions are maintained on the Client Access server, as shown in Figure 3.</span></span> <span data-ttu-id="77b00-231">Nas versões do Exchange posteriores ao Exchange 2010, as assinaturas são mantidas no servidor de caixa de correio, conforme mostrado na Figura 4.</span><span class="sxs-lookup"><span data-stu-id="77b00-231">In versions of Exchange later than Exchange 2010, subscriptions are maintained on the Mailbox server, as shown in Figure 4.</span></span>
  
<span data-ttu-id="77b00-232">**Figura 3. Processo de manutenção da afinidade no Exchange 2010**</span><span class="sxs-lookup"><span data-stu-id="77b00-232">**Figure 3. Process for maintaining affinity in Exchange 2010**</span></span>

![An illustration that shows how the table of active subscriptions is maintained on the Client Access server in Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
<span data-ttu-id="77b00-234">**Figura 4. Processo para manter a afinidade no Exchange Online e no Exchange 2013**</span><span class="sxs-lookup"><span data-stu-id="77b00-234">**Figure 4. Process for maintaining affinity in Exchange Online and Exchange 2013**</span></span>

![An illustration that shows how the load balancer and the Client Access server route requests to the mailbox server that maintains the table of active subscriptions in Exchange Server and Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
<span data-ttu-id="77b00-236">No Exchange 2010, o cliente só conhece o endereço do balanceador de carga e o exchangecookie retornado pelo servidor garante que a solicitação seja encaminhada para o servidor de acesso para cliente certo.</span><span class="sxs-lookup"><span data-stu-id="77b00-236">In Exchange 2010, the client only knows the address of the load balancer, and the exchangecookie that is returned by the server ensures that the request is routed to the right Client Access server.</span></span> <span data-ttu-id="77b00-237">No entanto, em versões posteriores, as funções de servidor de acesso para cliente e o balanceador de carga devem rotear as solicitações apropriadamente antes de chegarem ao servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77b00-237">However, in later versions, the load balancer and the Client Access server roles both have to route the requests appropriately before they get to the Mailbox server.</span></span> <span data-ttu-id="77b00-238">Para fazer isso, são necessárias informações adicionais, que é o motivo pelo qual os novos cabeçalhos e cookie foram introduzidos.</span><span class="sxs-lookup"><span data-stu-id="77b00-238">To do that, additional information is required, which is why the new headers and cookie were introduced.</span></span> <span data-ttu-id="77b00-239">O artigo [inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explica como as assinaturas são mantidas no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="77b00-239">The article [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explains how subscriptions are maintained in Exchange 2013.</span></span> 
  
<span data-ttu-id="77b00-240">Você pode notar que o exchangecookie que o Exchange 2010 usa ainda é retornado por versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="77b00-240">You might notice that the exchangecookie that Exchange 2010 uses is still returned by later versions.</span></span> <span data-ttu-id="77b00-241">Não há danos em incluir esse cookie em solicitações, mas as versões posteriores do Exchange o ignoram.</span><span class="sxs-lookup"><span data-stu-id="77b00-241">There's no harm in including this cookie in requests, but later versions of Exchange ignore it.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="77b00-242">Confira também</span><span class="sxs-lookup"><span data-stu-id="77b00-242">See also</span></span>

- [<span data-ttu-id="77b00-243">Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-243">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [<span data-ttu-id="77b00-244">Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-244">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="77b00-245">Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-245">Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="77b00-246">Tratamento de erros relacionados à notificação no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-246">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
- [<span data-ttu-id="77b00-247">Alterações no gerenciamento da afinidade de assinaturas do EWS...</span><span class="sxs-lookup"><span data-stu-id="77b00-247">Changes in Managing Affinity for EWS Subscriptions…</span></span>](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [<span data-ttu-id="77b00-248">Limitação do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77b00-248">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

