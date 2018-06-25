---
title: Rotear as solicitações de hierarquia de pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Todas as solicitações de informações de pasta pública que requerem conhecimento da hierarquia de pasta pública, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteado para a caixa de correio de hierarquia de pasta pública de padrão para o usuário determinado. Para rotear as solicitações para essa caixa de correio, você precisará definir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox para especificar os valores retornados pelo serviço de descoberta automática.
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750826"
---
# <a name="route-public-folder-hierarchy-requests"></a><span data-ttu-id="f9215-104">Rotear as solicitações de hierarquia de pasta pública</span><span class="sxs-lookup"><span data-stu-id="f9215-104">Route public folder hierarchy requests</span></span>

<span data-ttu-id="f9215-105">Todas as solicitações de informações de pasta pública que requerem conhecimento da hierarquia de pasta pública, como mover, atualizar, excluir ou localizar pastas públicas, precisam ser roteado para a caixa de correio de hierarquia de pasta pública de padrão para o usuário determinado.</span><span class="sxs-lookup"><span data-stu-id="f9215-105">All requests for public folder information that require knowledge of the public folder hierarchy, such as moving, updating, deleting, or finding public folders, need to be routed to the default public folder hierarchy mailbox for the given user.</span></span> <span data-ttu-id="f9215-106">Para rotear as solicitações para essa caixa de correio, você precisará definir os cabeçalhos **X-AnchorMailbox** e **X-PublicFolderMailbox** para especificar os valores retornados pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f9215-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values returned by the Autodiscover service.</span></span> 
  
<span data-ttu-id="f9215-107">**Visão geral de pastas públicas**</span><span class="sxs-lookup"><span data-stu-id="f9215-107">**Overview of public folders**</span></span>

|<span data-ttu-id="f9215-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9215-108">Header</span></span>|<span data-ttu-id="f9215-109">O que é necessário?</span><span class="sxs-lookup"><span data-stu-id="f9215-109">What do I need?</span></span>|<span data-ttu-id="f9215-110">Como obtê-lo?</span><span class="sxs-lookup"><span data-stu-id="f9215-110">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f9215-111">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="f9215-111">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="f9215-112">O valor de [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) de uma resposta de descoberta automática SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) , que se torna o valor do cabeçalho **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-112">The [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value from a [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) Autodiscover SOAP response, which becomes the value of the **X-AnchorMailbox** header.</span></span><br/><br/> <span data-ttu-id="f9215-113">![TAREFAS PENDENTES](media/Ex15_PF_PFH_Anchor.png)</span><span class="sxs-lookup"><span data-stu-id="f9215-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span></span>| <span data-ttu-id="f9215-114">1. envie uma solicitação de **GetUserSetting** com o endereço SMTP da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9215-114">1. Send a **GetUserSetting** request with the SMTP address for the user's mailbox.</span></span><br/><br/><span data-ttu-id="f9215-115">2. o valor do elemento **PublicFolderInformation** que o serviço de descoberta automática retorna o cache.</span><span class="sxs-lookup"><span data-stu-id="f9215-115">2. Cache the value of the **PublicFolderInformation** element that the Autodiscover service returns.</span></span> <span data-ttu-id="f9215-116">Isso pode ser um cache de uma chamada de descoberta automática existente no seu código, ou uma nova [chamada EWS Managed API GetUserSettings](#bk_getpfinfoewsma) ou uma [solicitação SOAP GetUserSettings](#bk_getpfinfoews).</span><span class="sxs-lookup"><span data-stu-id="f9215-116">This can be a cached from an existing Autodiscover call in your code, or a new [EWS Managed API GetUserSettings call](#bk_getpfinfoewsma) or a [GetUserSettings SOAP request](#bk_getpfinfoews).</span></span>  <br/><br/><span data-ttu-id="f9215-117">3. use o elemento **PublicFolderInformation** para preencher o valor do cabeçalho **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-117">3. Use the **PublicFolderInformation** element to populate the value of the **X-AnchorMailbox** header.</span></span> <span data-ttu-id="f9215-118">O valor do elemento **PublicFolderInformation** é um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="f9215-118">The value of the **PublicFolderInformation** element is an SMTP address.</span></span>  <br/> |
|<span data-ttu-id="f9215-119">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="f9215-119">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="f9215-120">O valor de [servidor](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) de uma [resposta de descoberta automática de POX](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), que se torna o valor do cabeçalho **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-120">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value from a [POX Autodiscover response](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), which becomes the value of the **X-PublicFolderMailbox** header.</span></span><br/><br/> <span data-ttu-id="f9215-121">![TAREFAS PENDENTES](media/Ex15_PF_PFH_PFMailbox.png)</span><span class="sxs-lookup"><span data-stu-id="f9215-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span></span>|<span data-ttu-id="f9215-122">1. o serviço de [call POX descoberta automática](#bk_makeautodrequest) usando o endereço de email **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-122">1. [Call the POX Autodiscover](#bk_makeautodrequest) service using the **X-AnchorMailbox** email address.</span></span>  <br/><br/><span data-ttu-id="f9215-123">2. use o elemento de **servidor** retornado pelo serviço de descoberta automática para preencher o valor do cabeçalho **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-123">2. Use the **Server** element returned by the Autodiscover service to populate the value of the **X-PublicFolderMailbox** header.</span></span> <span data-ttu-id="f9215-124">O valor do **X-PublicFolderMailbox** é um endereço SMTP onde o nome de usuário é um GUID.</span><span class="sxs-lookup"><span data-stu-id="f9215-124">The value of the **X-PublicFolderMailbox** is an SMTP address where the username is a GUID.</span></span>  <br/> |

<br/>

<span data-ttu-id="f9215-125">Após ter determinado os valores de cabeçalho, incluí-los [quando você faz solicitações de hierarquia de pasta pública](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="f9215-125">After you have determined the header values, include them [when you make public folder hierarchy requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="f9215-126">As etapas neste artigo são específicas para solicitações de hierarquia de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="f9215-126">The steps in this article are specific to public folder hierarchy requests.</span></span> <span data-ttu-id="f9215-127">Para determinar se a sua solicitação é uma hierarquia de pasta pública ou a solicitação de conteúdo, consulte [Roteamento solicitações de pasta pública](public-folder-access-with-ews-in-exchange.md#bk_routing).</span><span class="sxs-lookup"><span data-stu-id="f9215-127">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a><span data-ttu-id="f9215-128">Determinar o valor do cabeçalho X-AnchorMailbox usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="f9215-128">Determine the value of the X-AnchorMailbox header by using the EWS Managed API</span></span>
<span data-ttu-id="f9215-129"><a name="bk_getpfinfoewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f9215-129"></span></span>

<span data-ttu-id="f9215-130">Para recuperar o valor de [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) usando a API gerenciada de EWS, você pode armazenar em cache o valor do elemento **PublicFolderInformation** retorna uma chamada existente ao serviço de descoberta automática ou fazer uma nova chamada.</span><span class="sxs-lookup"><span data-stu-id="f9215-130">To retrieve the [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) value by using the EWS Managed API, you can either cache the value of the **PublicFolderInformation** element that an existing call to the Autodiscover service returns, or make a new call.</span></span> 
  
<span data-ttu-id="f9215-131">Se você estiver fazendo uma nova chamada, você pode [obter configurações de usuário usando a API gerenciada de EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[obter configurações de usuário usando a API gerenciada de EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) para seu código e, em seguida, chame o **GetUserSettings** de exemplo do método usando o código a seguir, que recupera somente o valor do elemento **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="f9215-131">If you're making a new call, you can [Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) to your code, and then call the **GetUserSettings** sample method by using the following code, which retrieves only the value of the **PublicFolderInformation** element.</span></span> <span data-ttu-id="f9215-132">Inclua o endereço SMTP do usuário da caixa de correio como um parâmetro de entrada.</span><span class="sxs-lookup"><span data-stu-id="f9215-132">Include the SMTP address of the mailbox user as an input parameter.</span></span> 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

<span data-ttu-id="f9215-133">Após a execução do código, as informações a seguir serão exibidas no console:</span><span class="sxs-lookup"><span data-stu-id="f9215-133">After running the code, the following information is displayed on the console:</span></span>
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

<span data-ttu-id="f9215-134">Agora que você tem o valor de **PublicFolderInformation** , incluí-lo como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="f9215-134">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a><span data-ttu-id="f9215-135">Determinar o valor do cabeçalho X-AnchorMailbox usando SOAP</span><span class="sxs-lookup"><span data-stu-id="f9215-135">Determine the value of the X-AnchorMailbox header using SOAP</span></span>
<span data-ttu-id="f9215-136"><a name="bk_getpfinfoews"> </a></span><span class="sxs-lookup"><span data-stu-id="f9215-136"></span></span>

<span data-ttu-id="f9215-137">O exemplo de código a seguir mostra como recuperar o valor de **PublicFolderInformation** usando a operação de SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f9215-137">The following code example shows how to retrieve the **PublicFolderInformation** value by using the [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP operation.</span></span> <span data-ttu-id="f9215-138">O usuário de caixa de correio for especificado no elemento de [caixa de correio](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) e o elemento [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) limita a resposta para o valor de [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f9215-138">The mailbox user is specified in the [Mailbox](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) element, and the [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) element limits the response to the [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f9215-139">A resposta inclui o valor de **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="f9215-139">The response includes the **PublicFolderInformation** value.</span></span> 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

<span data-ttu-id="f9215-140">Agora que você tem o valor de **PublicFolderInformation** , incluí-lo como o valor para o cabeçalho X-AnchorMailbox em todas as solicitações de hierarquia de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="f9215-140">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a><span data-ttu-id="f9215-141">Fazer uma solicitação de descoberta automática para determinar o valor X-PublicFolderInformation</span><span class="sxs-lookup"><span data-stu-id="f9215-141">Make an Autodiscover request to determine the X-PublicFolderInformation value</span></span>
<span data-ttu-id="f9215-142"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="f9215-142"></span></span>

<span data-ttu-id="f9215-143">Fazer uma solicitação de descoberta automática usando o endereço de SMTP **PublicFolderInformation** , que agora está sendo usado como o valor **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-143">Make an Autodiscover request by using the **PublicFolderInformation** SMTP address, which is now being used as the **X-AnchorMailbox** value.</span></span> <span data-ttu-id="f9215-144">Use o [Exchange 2013: obter configurações de usuário com a descoberta automática](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) amostra de código para chamar o serviço de descoberta automática, porque ele simplifica o processo de descoberta automática para você.</span><span class="sxs-lookup"><span data-stu-id="f9215-144">Use the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="f9215-145">Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de descoberta automática de POX no endereço SMTP **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="f9215-145">This code sample uses the command line arguments listed in the following table to call the POX Autodiscover service on the **PublicFolderInformation** SMTP address.</span></span> 
  
|<span data-ttu-id="f9215-146">**Argumento da linha de comando**</span><span class="sxs-lookup"><span data-stu-id="f9215-146">**Command-line argument**</span></span>|<span data-ttu-id="f9215-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9215-147">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9215-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f9215-148">emailAddress</span></span>  <br/> |<span data-ttu-id="f9215-149">O endereço de **PublicFolderInformation** SMTP.</span><span class="sxs-lookup"><span data-stu-id="f9215-149">The **PublicFolderInformation** SMTP address.</span></span>  <br/> |
|<span data-ttu-id="f9215-150">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="f9215-150">-skipSOAP</span></span>  <br/> | <span data-ttu-id="f9215-151">Use as solicitações de descoberta automática de POX para este cenário.</span><span class="sxs-lookup"><span data-stu-id="f9215-151">Use POX Autodiscover requests for this scenario.</span></span>  <br/> |
|<span data-ttu-id="f9215-152">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f9215-152">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="f9215-153">Endereço de email do usuário da caixa de correio, que é usado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f9215-153">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="f9215-154">Você será solicitado a inserir a senha do usuário da caixa de correio quando você executa o exemplo.</span><span class="sxs-lookup"><span data-stu-id="f9215-154">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="f9215-155">Por exemplo, quando SharedPublicFolder@contoso.com é o endereço SMTP do elemento **PublicFolderInformation** e sonyaf@contoso.com é o usuário de caixa de correio, os argumentos de linha de comando devem estar no formato.</span><span class="sxs-lookup"><span data-stu-id="f9215-155">For example, when SharedPublicFolder@contoso.com is the SMTP address of the **PublicFolderInformation** element, and sonyaf@contoso.com is the mailbox user, the command-line arguments should look like this.</span></span> 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="f9215-156">Quando você executa o **Exchange 2013: obter configurações de usuário com a descoberta automática** amostra, a última resposta da descoberta automática deve ter êxito e incluir todas as configurações de usuário associadas a GUID de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f9215-156">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="f9215-157">O valor do [servidor](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) associado ao elemento de [protocolo](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)EXCH[tipo](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) é o valor de cabeçalho **X-PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="f9215-157">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value associated with the EXCH [Protocol](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)[Type](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) element is the **X-PublicFolderInformation** header value.</span></span> 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

<span data-ttu-id="f9215-158">Como alternativa, se você não quiser usar o **Exchange 2013: obter configurações de usuário com a descoberta automática** amostra, você pode obter o valor do **servidor** [gerando uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e, em seguida, enviando a seguir Autodiscover POX solicitação de cada URL até receber uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f9215-158">Alternatively, if you do not want to use the **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **Server** value by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span> <span data-ttu-id="f9215-159">SharedPublicFolder@contoso.com é o valor do cabeçalho **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="f9215-159">SharedPublicFolder@contoso.com is the value of the **X-PublicFolderMailbox** header.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="f9215-160">Para obter mais informações sobre o processo de descoberta automática, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md), [gerar uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e [descoberta automática do Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f9215-160">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="f9215-161">Defina os valores dos cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="f9215-161">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="f9215-162"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="f9215-162"></span></span>

<span data-ttu-id="f9215-163">Usando o valor do endereço **PublicFolderInformation** SMTP adquirido em [determinar o valor do cabeçalho X-AnchorMailbox usando a API gerenciada de EWS](#bk_getpfinfoewsma) ou [determinar o valor do cabeçalho X-AnchorMailbox usando SOAP](#bk_getpfinfoews) e o servidor ** **valor adquirido em [tornar uma solicitação de descoberta automática para determinar o valor X-PublicFolderInformation](#bk_makeautodrequest), defina os valores dos cabeçalhos **X-AnchorMailbox** e **X-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="f9215-163">Using the value of the **PublicFolderInformation** SMTP address acquired in [Determine the value of the X-AnchorMailbox header by using the EWS Managed API](#bk_getpfinfoewsma) or [Determine the value of the X-AnchorMailbox header using SOAP](#bk_getpfinfoews) and the **Server** value acquired in [Make an Autodiscover request to determine the X-PublicFolderInformation value](#bk_makeautodrequest), set the values of **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="f9215-164">Por exemplo, devido a um endereço de **PublicFolderInformation** SMTP do SharedPublicFolder@contoso.com e o valor de um **servidor** de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, inclua os seguintes cabeçalhos ao fazer chamadas para o seguinte métodos ou operações.</span><span class="sxs-lookup"><span data-stu-id="f9215-164">For example, given a **PublicFolderInformation** SMTP address of SharedPublicFolder@contoso.com and a **Server** value of 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, include the following headers when making calls to the following methods or operations.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

<span data-ttu-id="f9215-165">**Chamadas de pasta pública que exigem os cabeçalhos X-AnchorMailbox e X-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="f9215-165">**Public folder calls that require the X-AnchorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="f9215-166">**Métodos de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="f9215-166">**EWS Managed API methods**</span></span>|<span data-ttu-id="f9215-167">**Operações de EWS**</span><span class="sxs-lookup"><span data-stu-id="f9215-167">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9215-168">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="f9215-168">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="f9215-169">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="f9215-169">Folder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="f9215-170">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="f9215-170">Folder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="f9215-171">Folder.Move</span><span class="sxs-lookup"><span data-stu-id="f9215-171">Folder.Move</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f9215-172">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f9215-172">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="f9215-173">FindFolder</span><span class="sxs-lookup"><span data-stu-id="f9215-173">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="f9215-174">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f9215-174">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="f9215-175">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f9215-175">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="f9215-176">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="f9215-176">MoveFolder</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="f9215-177">Para adicionar esses cabeçalhos usando a API gerenciada de EWS, use o método [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f9215-177">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

<span data-ttu-id="f9215-178">Por exemplo, o código a seguir mostra uma solicitação [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) com o cabeçalho **X-AnchorMailbox** e **X-PublicFolderMailbox** definido para os valores recuperados nos exemplos neste artigo.</span><span class="sxs-lookup"><span data-stu-id="f9215-178">For example, the following code shows a [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f9215-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9215-179">See also</span></span>

- [<span data-ttu-id="f9215-180">Acessar pastas públicas com EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f9215-180">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="f9215-181">Rotear as solicitações de conteúdo de pasta pública</span><span class="sxs-lookup"><span data-stu-id="f9215-181">Route public folder content requests</span></span>](how-to-route-public-folder-content-requests.md)    
- [<span data-ttu-id="f9215-182">Obter configurações de usuário usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="f9215-182">Get user settings by using the EWS Managed API</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

