---
title: Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Saiba mais sobre como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.
ms.openlocfilehash: 7cfbfb5cc19e092c37e3d48a7fcc4f27023516e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750740"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a><span data-ttu-id="6ec8d-103">Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-103">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>

<span data-ttu-id="6ec8d-104">Saiba mais sobre como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-104">Find out about maintaining the affinity between a group of subscriptions and the Mailbox server.</span></span>
  
<span data-ttu-id="6ec8d-105">Afinidade é a associação de uma sequência de mensagens de solicitação e resposta com um determinado servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-105">Affinity is the association of a sequence of request and response messages with a particular Mailbox server.</span></span> <span data-ttu-id="6ec8d-106">Para a maioria das funcionalidades no Exchange, afinidade é manipulada pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-106">For most functionality in Exchange, affinity is handled by the server.</span></span> <span data-ttu-id="6ec8d-107">Notificações, no entanto, são uma exceção.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-107">Notifications, however, are an exception.</span></span> <span data-ttu-id="6ec8d-108">O cliente é responsável por manter a afinidade com o servidor de caixa de correio para inscrições de notificação.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-108">The client is responsible for maintaining the affinity with the Mailbox server for notification subscriptions.</span></span> <span data-ttu-id="6ec8d-109">Este afinidade permite que o balanceador de carga e servidores de acesso para cliente entre o cliente e o servidor de inscrições de notificação de rota e relacionadas solicitações para o servidor de caixa de correio que mantém a assinatura.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-109">This affinity enables the load balancer and Client Access servers between the client and the server to route notification subscriptions and related requests to the Mailbox server that maintains the subscription.</span></span> <span data-ttu-id="6ec8d-110">Sem afinidade, a solicitação pode ser roteada para um servidor de caixa de correio diferente que não inclui as inscrições do cliente, que podem causar um erro de [ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-110">Without affinity, the request might get routed to a different Mailbox server that does not include the client's subscriptions, which can cause an [ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) error to be returned.</span></span> 
  
## <a name="how-is-affinity-maintained"></a><span data-ttu-id="6ec8d-111">Como a afinidade é mantida?</span><span class="sxs-lookup"><span data-stu-id="6ec8d-111">How is affinity maintained?</span></span>
<span data-ttu-id="6ec8d-112"><a name="bk_howmaintained"> </a></span><span class="sxs-lookup"><span data-stu-id="6ec8d-112"></span></span>

<span data-ttu-id="6ec8d-113">Afinidade no Exchange é baseadas em cookies.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-113">Affinity in Exchange is cookie based.</span></span> <span data-ttu-id="6ec8d-114">O cliente dispara a criação do cookie, incluindo cabeçalhos específicos na solicitação de assinatura e, em seguida, a resposta de assinatura conterá o cookie.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-114">The client triggers the creation of the cookie by including specific headers in the subscription request, and then the subscription response contains the cookie.</span></span> <span data-ttu-id="6ec8d-115">O cliente envia esse cookie nas solicitações subsequentes para garantir que a solicitação é roteada para o servidor de caixa de correio à direita.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-115">The client then sends that cookie in subsequent requests to ensure that the request is routed to the right Mailbox server.</span></span>
  
<span data-ttu-id="6ec8d-116">Mais especificamente, a afinidade no Exchange é tratada pelo seguinte:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-116">More specifically, affinity in Exchange is handled by the following:</span></span> 
  
- <span data-ttu-id="6ec8d-117">X-AnchorMailbox — Um cabeçalho HTTP, que está incluído na solicitação de assinatura inicial.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-117">X-AnchorMailbox — An HTTP header that is included in the initial subscription request.</span></span> <span data-ttu-id="6ec8d-118">Identifica a primeira caixa de correio em um grupo de caixas de correio que compartilham a afinidade com o mesmo servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-118">It identifies the first mailbox in a group of mailboxes that share affinity with the same Mailbox server.</span></span>
    
- <span data-ttu-id="6ec8d-119">X-PreferServerAffinity — Um cabeçalho HTTP que está incluído na solicitação de assinatura inicial com o cabeçalho X-AnchorMailbox e estiver definido como true para indicar que o cliente está solicitando que afinidade ser mantidas com o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-119">X-PreferServerAffinity — An HTTP header that is included in the initial subscription request with the X-AnchorMailbox header and is set to true to indicate that the client is requesting that affinity be maintained with the Mailbox server.</span></span>
    
- <span data-ttu-id="6ec8d-120">X-BackEndOverrideCookie — Um cookie que está incluído na resposta assinatura inicial e contém um cookie que o balanceador de carga e o servidor de acesso para cliente usam para rotear solicitações subsequentes no mesmo servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-120">X-BackEndOverrideCookie — A cookie that is included in the initial subscription response and contains a cookie that the load balancer and Client Access server use to route subsequent requests to the same Mailbox server.</span></span>
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a><span data-ttu-id="6ec8d-121">Como manter a afinidade usando a API gerenciada de EWS ou EWS?</span><span class="sxs-lookup"><span data-stu-id="6ec8d-121">How do I maintain affinity by using the EWS Managed API or EWS?</span></span>
<span data-ttu-id="6ec8d-122"><a name="bk_howdoimaintain"> </a></span><span class="sxs-lookup"><span data-stu-id="6ec8d-122"></span></span>

<span data-ttu-id="6ec8d-123">Você pode usar as mesmas etapas para manter a afinidade para diversas assinaturas de caixa de correio e de seus servidores de caixa de correio, não importa se você estiver usando o streaming, pull ou notificações de push, e independentemente se você está direcionando do Exchange no servidor local ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-123">You can use the same steps to maintain affinity for multiple mailbox subscriptions and their Mailbox servers, regardless of whether you are using streaming, pull, or push notifications, and regardless of whether you're targeting an Exchange on-premises server or Exchange Online.</span></span>
  
1. <span data-ttu-id="6ec8d-124">Para cada caixa de correio, [descoberta automática de chamadas](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e obtenha as configurações de usuário GroupingInformation e ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-124">For each mailbox, [call Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and get the GroupingInformation and ExternalEwsUrl user settings.</span></span> <span data-ttu-id="6ec8d-125">Para descoberta automática do SOAP, você usar o elemento de [configuração](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) e de descoberta automática POX, você usar o elemento [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6ec8d-125">For SOAP Autodiscover, you use the [Setting](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) element, and for POX Autodiscover, you use the [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) element.</span></span> 
    
2. <span data-ttu-id="6ec8d-126">Usando as configurações de GroupingInformation e ExternalEwsUrl entre as respostas de descoberta automática, caixas de correio local com o mesmo ExternalEwsUrl e GroupingInformation concatenado valor no mesmo grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-126">Using the GroupingInformation and ExternalEwsUrl settings from the Autodiscover responses, place mailboxes with the same ExternalEwsUrl and GroupingInformation concatenated value in the same group.</span></span> <span data-ttu-id="6ec8d-127">Se nenhum grupo tiver mais de 200 caixas de correio, se dividem os grupos de modo que cada grupo tenha não mais de 200 caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-127">If any groups have more than 200 mailboxes, break the groups down further so that each group has no more than 200 mailboxes.</span></span>
    
3. <span data-ttu-id="6ec8d-128">Criar e usar um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) para o restante do procedimento.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-128">Create and use one [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) object for the rest of the procedure.</span></span> <span data-ttu-id="6ec8d-129">Quando você usa o mesmo objeto **ExchangeService** , cookies e os cabeçalhos (quando eles estão definidos) são mantidos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-129">When you use the same **ExchangeService** object, cookies and headers (when they are set) are automatically maintained.</span></span> <span data-ttu-id="6ec8d-130">Observe que, se você não pretende inscrições de streaming de grupo em uma única conexão, você está livre para criar um objeto **ExchangeService** diferente para cada usuário representado.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-130">Note that if you do not intend to group streaming subscriptions into a single connection, you are free to create a different **ExchangeService** object for each impersonated user.</span></span> 
    
4. <span data-ttu-id="6ec8d-131">[Enviar uma assinatura de](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) solicitação para o usuário cujo nome de usuário aparece primeiro quando todos os usuários no grupo são classificados em ordem alfabética (vamos nos referir a esse usuário como o usuário de caixa de correio âncora).</span><span class="sxs-lookup"><span data-stu-id="6ec8d-131">[Send a subscription](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) request for the user whose user name appears first when all users in the group are sorted alphabetically (we'll refer to this user as the anchor mailbox user).</span></span> <span data-ttu-id="6ec8d-132">Faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-132">Do the following:</span></span> 
    
  - <span data-ttu-id="6ec8d-133">Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário da caixa de correio âncora.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-133">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user.</span></span>
    
  - <span data-ttu-id="6ec8d-134">Inclua o cabeçalho X-PreferServerAffinity com um conjunto de valor como true.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-134">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6ec8d-135">Use a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (o tipo de [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6ec8d-135">Use the [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
5. <span data-ttu-id="6ec8d-136">Em resposta a assinatura, obtenha o valor X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-136">In the subscription response, get the X-BackEndOverrideCookie value.</span></span> <span data-ttu-id="6ec8d-137">Inclua esse valor em cada uma das solicitações subsequentes de assinatura para os usuários deste grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-137">Include this value in each of the subsequent subscription requests for users in this group.</span></span>
    
6. <span data-ttu-id="6ec8d-138">Para cada usuário adicional no grupo, enviar uma solicitação de assinatura e faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-138">For each additional user in the group, send a subscription request and do the following:</span></span>
    
  - <span data-ttu-id="6ec8d-139">Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário âncora da caixa de correio para o grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-139">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user for the group.</span></span>
    
  - <span data-ttu-id="6ec8d-140">Inclua o cabeçalho X-PreferServerAffinity com um conjunto de valor como true.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-140">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6ec8d-141">Inclua o X-BackEndOverrideCookie foi retornado em resposta de assinatura do usuário de caixa de correio a âncora.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-141">Include the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response.</span></span>
    
  - <span data-ttu-id="6ec8d-142">Use a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (o tipo de [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6ec8d-142">Use the [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
    <span data-ttu-id="6ec8d-143">Observe que o servidor usará os valores de X-PreferServerAffinity e X-BackendOverrideCookie juntos para executar o roteamento para o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-143">Note that the server uses the X-PreferServerAffinity and X-BackendOverrideCookie values together to perform the routing to the mailbox server.</span></span> <span data-ttu-id="6ec8d-144">O cabeçalho X-AnchorMailbox também é necessário, mas é ignorado pelo servidor se os dois valores são válidos.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-144">The X-AnchorMailbox header is also required, but is ignored by the server if the other two values are valid.</span></span> <span data-ttu-id="6ec8d-145">Se X-AnchorMailbox e X-PreferServerAffinity estão em uma solicitação e X-BackendOverrideCookie não for incluído, o valor X-AnchorMailbox é usado para rotear solicitações.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-145">If X-AnchorMailbox and X-PreferServerAffinity are in a request and X-BackendOverrideCookie is not included, the X-AnchorMailbox value is used to route the requests.</span></span>
    
    <span data-ttu-id="6ec8d-146">Como o X-PreferServerAffinity e os valores de X-BackendOverrideCookie executam o roteamento, se a caixa de correio âncora nunca mover para outro servidor ou um grupo, a lógica não altera porque o X-BackendOverrideCookie roteará a solicitação ao servidor correto para o grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-146">Because the X-PreferServerAffinity and X-BackendOverrideCookie values perform the routing, if the anchor mailbox ever moves to another group or server, the logic does not change because the X-BackendOverrideCookie will route the request to the correct server for the group.</span></span>
    
7. <span data-ttu-id="6ec8d-147">Enviar solicitações de [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) ou de um único [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) para o grupo e faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-147">Send a single [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) requests for the group, and do the following:</span></span> 
    
  - <span data-ttu-id="6ec8d-148">Inclua os valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) retornados em cada uma das respostas a inscrição individual para caixas de correio no grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-148">Include the [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values returned in each of the individual subscription responses for mailboxes in the group.</span></span> 
    
  - <span data-ttu-id="6ec8d-149">Se mais de 200 assinaturas existirem para o grupo, criem várias solicitações.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-149">If more than 200 subscriptions exist for the group, create multiple requests.</span></span> <span data-ttu-id="6ec8d-150">O número máximo de valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) a serem incluídos em uma solicitação é 200.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-150">The maximum number of [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values to include in a request is 200.</span></span> 
    
  - <span data-ttu-id="6ec8d-151">Se você precisar de mais conexões que estão disponíveis para a caixa de correio de destino, use a conta de serviço para representar a caixa de correio para o grupo; âncora Caso contrário, não use a representação.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-151">If you need more connections than are available to the target mailbox, use the service account to impersonate the anchor mailbox for the group; otherwise, do not use impersonation.</span></span> <span data-ttu-id="6ec8d-152">O ideal é que você deseja representar uma caixa de correio exclusiva por solicitação [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) para que você nunca encontrar os limites de limitação.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-152">Ideally, you want to impersonate a unique mailbox per [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) request so that you never encounter throttling limits.</span></span> 
    
  - <span data-ttu-id="6ec8d-153">Use ApplicationImpersonation se precisar de [mais conexões que estão disponíveis para a caixa de correio de destino](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); Caso contrário, não use ApplicationImpersonation.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-153">Use ApplicationImpersonation if you need [more connections than are available to the target mailbox](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); otherwise, do not use ApplicationImpersonation.</span></span>
    
  - <span data-ttu-id="6ec8d-154">Incluir o cabeçalho X-PreferServerAffinity e defina-o como true.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-154">Include the X-PreferServerAffinity header and set it to true.</span></span> <span data-ttu-id="6ec8d-155">Esse valor é incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-155">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
  - <span data-ttu-id="6ec8d-156">Inclua o X-BackEndOverrideCookie para o grupo (o X-BackEndOverrideCookie retornado na resposta de assinatura do usuário da caixa de correio âncora).</span><span class="sxs-lookup"><span data-stu-id="6ec8d-156">Include the X-BackEndOverrideCookie for the group (the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response).</span></span> <span data-ttu-id="6ec8d-157">Esse valor é incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-157">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
8. <span data-ttu-id="6ec8d-158">Passe os eventos retornados para um thread separado para processamento.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-158">Pass the returned events to a separate thread for processing.</span></span>
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a><span data-ttu-id="6ec8d-159">Os valores de limitação para os quais é necessário levar em consideração?</span><span class="sxs-lookup"><span data-stu-id="6ec8d-159">What throttling values do I need to take into consideration?</span></span>
<span data-ttu-id="6ec8d-160"><a name="bk_throttling"> </a></span><span class="sxs-lookup"><span data-stu-id="6ec8d-160"></span></span>

<span data-ttu-id="6ec8d-161">Ao planejar a implementação de notificação, você vai querer leve em consideração as dois valores: o número de conexões e o número de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-161">As you plan your notification implementation, you'll want to take two values into consideration: the number of connections, and the number of subscriptions.</span></span> <span data-ttu-id="6ec8d-162">A tabela a seguir lista os valores padrão para cada configuração de [limitação](ews-throttling-in-exchange.md) e como as configurações são usadas.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-162">The following table lists the default values for each [throttling](ews-throttling-in-exchange.md) setting and how the settings are used.</span></span> <span data-ttu-id="6ec8d-163">Para cada valor, o orçamento é alocado para a caixa de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-163">For each value, the budget is allocated to the target mailbox.</span></span> <span data-ttu-id="6ec8d-164">Por esse motivo, usando a representação para obter conexões adicionais é uma etapa necessária em muitos cenários.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-164">For this reason, using impersonation to gain additional connections is a required step in many scenarios.</span></span> 
  
<span data-ttu-id="6ec8d-165">**Tabela 1. Limitação de valores padrão**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-165">**Table 1. Default throttling values**</span></span>

|<span data-ttu-id="6ec8d-166">**Área de consideração**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-166">**Area of consideration**</span></span>|<span data-ttu-id="6ec8d-167">**Configuração de limitação**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-167">**Throttling setting**</span></span>|<span data-ttu-id="6ec8d-168">**Default value**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-168">**Default value**</span></span>|<span data-ttu-id="6ec8d-169">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-169">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="6ec8d-170">Conexões de streaming</span><span class="sxs-lookup"><span data-stu-id="6ec8d-170">Streaming connections</span></span>  <br/> |<span data-ttu-id="6ec8d-171">Padrão deslocado limite de conexão</span><span class="sxs-lookup"><span data-stu-id="6ec8d-171">Default hanging connection limit</span></span>  <br/> |<span data-ttu-id="6ec8d-172">10 para Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6ec8d-172">10 for Exchange Online</span></span>  <br/> <span data-ttu-id="6ec8d-173">3 para Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6ec8d-173">3 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6ec8d-174">O número máximo de conexões simultâneas de streaming que uma conta pode ter abertos no servidor ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-174">The maximum number of concurrent streaming connections that an account can have open on the server at one time.</span></span> <span data-ttu-id="6ec8d-175">Para trabalhar nesse limite, use uma conta de serviço com a função ApplicationImpersonation atribuída para as caixas de correio de destino e representar o primeiro usuário em cada grupo de ID de assinatura quando obtendo transmitidas eventos.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-175">To work within this limit, use a service account with the ApplicationImpersonation role assigned for the target mailboxes, and impersonate the first user in each subscription ID group when getting streamed events.</span></span>  <br/> |
|<span data-ttu-id="6ec8d-176">Conexões de recepção ou de envio</span><span class="sxs-lookup"><span data-stu-id="6ec8d-176">Pull or push connections</span></span>  <br/> |<span data-ttu-id="6ec8d-177">EWSMaxConcurrency</span><span class="sxs-lookup"><span data-stu-id="6ec8d-177">EWSMaxConcurrency</span></span>  <br/> |<span data-ttu-id="6ec8d-178">27</span><span class="sxs-lookup"><span data-stu-id="6ec8d-178">27</span></span>  <br/> |<span data-ttu-id="6ec8d-179">O número máximo de conexões simultâneas de recepção ou de envio (solicitações que foram recebidas, mas ainda não respondidas) que uma conta pode ter abertas no servidor ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-179">The maximum number of concurrent pull or push connections (requests that have been received but not yet responded to) that an account can have open on the server at one time.</span></span>  <br/> |
|<span data-ttu-id="6ec8d-180">Assinaturas</span><span class="sxs-lookup"><span data-stu-id="6ec8d-180">Subscriptions</span></span>  <br/> |<span data-ttu-id="6ec8d-181">EWSMaxSubscriptions</span><span class="sxs-lookup"><span data-stu-id="6ec8d-181">EWSMaxSubscriptions</span></span>  <br/> |<span data-ttu-id="6ec8d-182">20 para o Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6ec8d-182">20 for Exchange Online</span></span>  <br/> <span data-ttu-id="6ec8d-183">5000 para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6ec8d-183">5000 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6ec8d-184">O número máximo de inscrições nonexpired que uma conta pode ter ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-184">The maximum number of nonexpired subscriptions that an account can have at one time.</span></span> <span data-ttu-id="6ec8d-185">Esse valor é diminuído quando a assinatura é criada no servidor.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-185">This value is decremented when the subscription is created on the server.</span></span>  <br/> |
   
<span data-ttu-id="6ec8d-186">O exemplo a seguir mostra como os orçamentos são manipulados entre qualquer caixa de correio de destino e a conta de serviço que possui a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) atribuída para as caixas de correio de destino.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-186">The following example shows how budgets are handled between any target mailbox and the service account that has the [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) role assigned for the target mailboxes.</span></span> 
  
- <span data-ttu-id="6ec8d-187">ServiceAccount1 (sa1) personifica muitos usuários (m1, m2, m3 e assim por diante) e cria assinaturas para cada caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-187">ServiceAccount1 (sa1) impersonates many users (m1, m2, m3, and so on) and creates subscriptions for each mailbox.</span></span> <span data-ttu-id="6ec8d-188">Observe que, quando as assinaturas são criadas, o proprietário da assinatura é sa1, portanto, quando sa1 abre uma conexão com as assinaturas, EWS impõe que as assinaturas pertencentes sa1.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-188">Note that when the subscriptions are created, the subscription owner is sa1, so when sa1 opens a connection with the subscriptions, EWS enforces that the subscriptions are owned by sa1.</span></span>
    
- <span data-ttu-id="6ec8d-189">Sa1 pode abrir a conexão das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-189">Sa1 can open the connection in the following ways:</span></span>
    
1. <span data-ttu-id="6ec8d-190">Sem representação, portanto a conexão é cobrado contra sa1.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-190">Without impersonation, so the connection is charged against sa1.</span></span>
    
2. <span data-ttu-id="6ec8d-191">Ao representar qualquer um dos usuários — m1, por exemplo — para que a conexão é cobrado contra uma cópia do orçamento do m1.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-191">By impersonating any of the users — m1 for example — so that the connection is charged against a copy of m1's budget.</span></span> <span data-ttu-id="6ec8d-192">(M1 próprio pode abrir dez conexões usando o Exchange Online e todas as contas de serviço as representação m1 podem abrir dez conexões usando o orçamento copiado.)</span><span class="sxs-lookup"><span data-stu-id="6ec8d-192">(M1 itself can open ten connections by using Exchange Online, and all service accounts impersonating m1 can open ten connections by using the copied budget.)</span></span>
    
- <span data-ttu-id="6ec8d-193">Se for atingido o limite de conexão, as seguintes soluções alternativas estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="6ec8d-193">If the connection limit is hit, the following workarounds are available:</span></span>
    
  - <span data-ttu-id="6ec8d-194">Se a opção 1 é usada, o administrador pode criar várias contas de serviço para representar usuários adicionais.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-194">If option 1 is used, the administrator can create multiple service accounts to impersonate additional users.</span></span>
    
  - <span data-ttu-id="6ec8d-195">Se a opção 2 é usada, o código pode representar outro usuário — m2 por exemplo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-195">If option 2 is used, the code can impersonate another user — m2 for example.</span></span>
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a><span data-ttu-id="6ec8d-196">Exemplo: Mantendo afinidade entre um grupo de assinaturas e o servidor de caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6ec8d-196">Example: Maintaining affinity between a group of subscriptions and the Mailbox server</span></span>
<span data-ttu-id="6ec8d-197"><a name="bk_ce"> </a></span><span class="sxs-lookup"><span data-stu-id="6ec8d-197"></span></span>

<span data-ttu-id="6ec8d-198">Okey, vamos vê-lo em ação.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-198">Okay, let's see it in action.</span></span> <span data-ttu-id="6ec8d-199">O exemplo de código a seguir mostra como agrupar usuários e usar os cabeçalhos X-AnchorMailbox e PreferServerAffinity-X e o cookie de X-BackendOverrideCookie para manter a afinidade com o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-199">The following code example shows you how to group users and use the X-AnchorMailbox and X-PreferServerAffinity headers and the X-BackendOverrideCookie cookie to maintain affinity with the Mailbox server.</span></span> <span data-ttu-id="6ec8d-200">Como os cabeçalhos e o cookie são de importância principal no bloco afinidade, este exemplo enfoca as EWS XML solicitações e respostas.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-200">Because the headers and the cookie are of primary importance in the affinity story, this example focuses on the EWS XML requests and responses.</span></span> <span data-ttu-id="6ec8d-201">Para usar a API gerenciada de EWS para criar o corpo das solicitações de inscrição e respostas, consulte [notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) e [receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="6ec8d-201">To use the EWS Managed API to create the body of the subscription requests and responses, see [Stream notifications about mailbox events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) and [Pull notifications about mailbox events by using EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6ec8d-202">Esta seção inclui etapas adicionais que sejam específicos para manutenção afinidade e adicionando os cabeçalhos às suas solicitações.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-202">This section includes additional steps particular to maintaining affinity and adding the headers to your requests.</span></span>
  
<span data-ttu-id="6ec8d-203">Este exemplo tem quatro usuários: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com e sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-203">This example has four users: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com, and sadie@contoso.com.</span></span> <span data-ttu-id="6ec8d-204">A figura a seguir mostra os GroupingInformation e ExternalEwsUrl [configurações de descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) para os usuários.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-204">The following figure shows the GroupingInformation and ExternalEwsUrl [Autodiscover settings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) for the users.</span></span> 
  
<span data-ttu-id="6ec8d-205">**Figura 1. Usado para caixas de correio do grupo de definições de descoberta automática**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-205">**Figure 1. Autodiscover settings used to group mailboxes**</span></span>

![A table that shows the GroupingInformation and ExternalEwsUrl values for each of the users.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
<span data-ttu-id="6ec8d-207">Usando as configurações das respostas de descoberta automática, as caixas de correio são agrupadas pelo valor concatenado das configurações de GroupingInformation e ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-207">Using the settings from the Autodiscover responses, the mailboxes are grouped by the concatenated value of the GroupingInformation and ExternalEwsUrl settings.</span></span> <span data-ttu-id="6ec8d-208">Neste exemplo, Alfredo e Sadie tem os mesmos valores, para que eles estão em um grupo e Alisa e Ronnie compartilham os mesmos valores, portanto, eles estão em outro grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-208">In this example, Alfred and Sadie have the same values, so they are in one group, and Alisa and Ronnie share the same values, so they are in another group.</span></span>
  
<span data-ttu-id="6ec8d-209">**Figura 2. Criação de grupos de caixa de correio**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-209">**Figure 2. Creating mailbox groups**</span></span>

![A table that shows how mailbox groups are created using Autodiscover settings.](media/Exchange2013_NotificationAffinityGrouping.png)
  
<span data-ttu-id="6ec8d-211">Neste exemplo, para fins de focaremos na grupo. Podemos seria usar as mesmas etapas para o grupo B, mas use um valor diferente de X-AnchorMailbox para esse grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-211">For the purpose of this example, we'll focus on Group A. We would use the same steps for group B, but use a different X-AnchorMailbox value for that group.</span></span>
  
<span data-ttu-id="6ec8d-212">Usando [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx), crie a solicitação de inscrição para a caixa de correio âncora (alfred@contoso.com), com o cabeçalho X-AnchorMailbox definido como o seu endereço de email e um valor de cabeçalho X-PreferServerAffinity verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-212">Using [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx), create the subscription request for the anchor mailbox (alfred@contoso.com), with the X-AnchorMailbox header set to the their email address and an X-PreferServerAffinity header value of true.</span></span> <span data-ttu-id="6ec8d-213">Configurar esses valores de dois cabeçalho irá disparar o servidor para criar um X-BackEndOverrideCookie para a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-213">Setting these two header values will trigger the server to create an X-BackEndOverrideCookie for the response.</span></span>
  
<span data-ttu-id="6ec8d-214">Se você estiver usando o EWS Managed API, use o método[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e) de [HttpHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)para adicionar os dois cabeçalhos à sua solicitação de assinatura, como mostrado.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-214">If you're using the EWS Managed API, use the [HttpHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e) method to add the two headers to your subscription request, as shown.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

<span data-ttu-id="6ec8d-215">Portanto solicitação de assinatura de Alfredo tem esta aparência.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-215">So Alfred's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="6ec8d-216">A seguinte mensagem XML é a resposta à solicitação de assinatura de Alfredo e inclui o X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-216">The following XML message is the response to Alfred's subscription request, and it includes the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6ec8d-217">Reenvie esse cookie para todas as solicitações subsequentes para os usuários deste grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-217">Resend this cookie for all subsequent requests for users in this group.</span></span> <span data-ttu-id="6ec8d-218">Observe que a resposta também contém cookies adicionais, como o cookie exchangecookie usados pelo Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-218">Notice that the response also contains additional cookies, such as the exchangecookie cookie used by Exchange 2010.</span></span> <span data-ttu-id="6ec8d-219">O Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013, ignorar exchangecookie se ela estiver incluída nas solicitações de inscrição subsequentes.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-219">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013, ignore exchangecookie if it is included in subsequent subscription requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="6ec8d-220">Usando o X-BackEndOverrideCookie da resposta de Alfredo e cabeçalho X-AnchorMailbox, a solicitação de assinatura é criada para Sadie, o outro membro da solicitação de assinatura do grupo A. Sadie tem esta aparência.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-220">Using the X-BackEndOverrideCookie from Alfred's response and the X-AnchorMailbox header, the subscription request is created for Sadie, the other member of Group A. Sadie's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@consoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@consoso.com </t:SmtpAddress>
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

<span data-ttu-id="6ec8d-221">Resposta de assinatura de Sadie tem esta aparência.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-221">Sadie's subscription response looks like this.</span></span> <span data-ttu-id="6ec8d-222">Observe que ele não inclui o X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-222">Note that it does not include the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6ec8d-223">O cliente é responsável para armazenar em cache o valor em solicitações futuras.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-223">The client is responsible for caching that value for future requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="6ec8d-224">Usando os valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) entre as respostas de inscrição, uma solicitação de operação [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) foi criada para todas as assinaturas no grupo.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-224">Using the [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values from the subscription responses, a [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) operation request was created for all the subscriptions in the group.</span></span> <span data-ttu-id="6ec8d-225">Como há menos de 200 assinaturas nesse grupo, eles são todos enviados em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-225">Because there are less than 200 subscriptions in this group, they are all sent in one request.</span></span> <span data-ttu-id="6ec8d-226">O cabeçalho X-PreferServerAffinity estiver definido como true e o X-BackEndOverrideCookie está incluído.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-226">The X-PreferServerAffinity header is set to true and the X-BackEndOverrideCookie is included.</span></span> 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="6ec8d-227">Os eventos retornados serão então passados a um segmento separado para processamento.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-227">The returned events are then passed to a separate thread for processing.</span></span>
  
## <a name="how-has-affinity-changed"></a><span data-ttu-id="6ec8d-228">Como a afinidade mudou?</span><span class="sxs-lookup"><span data-stu-id="6ec8d-228">How has affinity changed?</span></span>
<span data-ttu-id="6ec8d-229"><a name="bk_howchanged"> </a></span><span class="sxs-lookup"><span data-stu-id="6ec8d-229"></span></span>

<span data-ttu-id="6ec8d-230">No Exchange 2010, as assinaturas são mantidas no servidor de acesso para cliente, conforme mostrado na Figura 3.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-230">In Exchange 2010, subscriptions are maintained on the Client Access server, as shown in Figure 3.</span></span> <span data-ttu-id="6ec8d-231">Nas versões do Exchange mais recente do que o Exchange 2010, as assinaturas são mantidas no servidor de caixa de correio, conforme mostrado na Figura 4.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-231">In versions of Exchange later than Exchange 2010, subscriptions are maintained on the Mailbox server, as shown in Figure 4.</span></span>
  
<span data-ttu-id="6ec8d-232">**Figura 3. Processo para manter a afinidade no Exchange 2010**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-232">**Figure 3. Process for maintaining affinity in Exchange 2010**</span></span>

![An illustration that shows how the table of active subscriptions is maintained on the Client Access server in Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
<span data-ttu-id="6ec8d-234">**Figura 4. Processo para manter a afinidade no Exchange Online e Exchange 2013**</span><span class="sxs-lookup"><span data-stu-id="6ec8d-234">**Figure 4. Process for maintaining affinity in Exchange Online and Exchange 2013**</span></span>

![An illustration that shows how the load balancer and the Client Access server route requests to the mailbox server that maintains the table of active subscriptions in Exchange Server and Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
<span data-ttu-id="6ec8d-236">No Exchange 2010, o cliente só sabe o endereço do balanceador de carga e o exchangecookie que é retornado pelo servidor garante que a solicitação é roteada para o servidor de acesso para cliente à direita.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-236">In Exchange 2010, the client only knows the address of the load balancer, and the exchangecookie that is returned by the server ensures that the request is routed to the right Client Access server.</span></span> <span data-ttu-id="6ec8d-237">No entanto, em versões posteriores, o balanceador de carga e as funções de servidor acesso para cliente ter que rotear solicitações apropriadamente que eles cheguem ao servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-237">However, in later versions, the load balancer and the Client Access server roles both have to route the requests appropriately before they get to the Mailbox server.</span></span> <span data-ttu-id="6ec8d-238">Para fazer o que, forem necessárias informações adicionais, que é o motivo pelo qual os novos cabeçalhos e cookie introduzidas.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-238">To do that, additional information is required, which is why the new headers and cookie were introduced.</span></span> <span data-ttu-id="6ec8d-239">O artigo [inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explica como as assinaturas são mantidas no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-239">The article [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explains how subscriptions are maintained in Exchange 2013.</span></span> 
  
<span data-ttu-id="6ec8d-240">Você pode observar que o exchangecookie que usa o Exchange 2010 ainda será retornada por versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-240">You might notice that the exchangecookie that Exchange 2010 uses is still returned by later versions.</span></span> <span data-ttu-id="6ec8d-241">Não há nenhuma danos esse cookie, incluindo solicitações de, mas as versões anteriores do Exchange ignorá-la.</span><span class="sxs-lookup"><span data-stu-id="6ec8d-241">There's no harm in including this cookie in requests, but later versions of Exchange ignore it.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6ec8d-242">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ec8d-242">See also</span></span>

- [<span data-ttu-id="6ec8d-243">Inscrições de notificação, eventos de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-243">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [<span data-ttu-id="6ec8d-244">Notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-244">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6ec8d-245">Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-245">Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6ec8d-246">Tratando erros relacionados a notificação no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-246">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
- [<span data-ttu-id="6ec8d-247">Alterações no gerenciamento de afinidade de assinaturas do EWS...</span><span class="sxs-lookup"><span data-stu-id="6ec8d-247">Changes in Managing Affinity for EWS Subscriptions…</span></span>](http://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [<span data-ttu-id="6ec8d-248">EWS limitação no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ec8d-248">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

