---
title: Manipulação de mensagens de erro de descoberta automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750666"
---
# <a name="handling-autodiscover-error-messages"></a><span data-ttu-id="6012d-103">Manipulação de mensagens de erro de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6012d-103">Handling Autodiscover error messages</span></span>

<span data-ttu-id="6012d-104">Saiba mais sobre os diferentes tipos de erros de descoberta automática e o que fazer com eles.</span><span class="sxs-lookup"><span data-stu-id="6012d-104">Learn about the different types of Autodiscover errors and what to do with them.</span></span>
  
<span data-ttu-id="6012d-105">Descoberta automática permite que seus aplicativos recuperar informações de configuração automaticamente, e ele funciona bem.</span><span class="sxs-lookup"><span data-stu-id="6012d-105">Autodiscover enables your applications to retrieve configuration information automatically, and it works great.</span></span> <span data-ttu-id="6012d-106">No entanto, nem sempre tudo de acordo com o plano.</span><span class="sxs-lookup"><span data-stu-id="6012d-106">However, things don't always go according to plan.</span></span> <span data-ttu-id="6012d-107">Vejamos os erros comuns que podem ocorrer e como você pode tratá-los para minimizar a necessidade de avisar o usuário configurar manualmente o cliente.</span><span class="sxs-lookup"><span data-stu-id="6012d-107">Let's look at the common errors that might occur and how you can handle them to minimize the need to prompt your user to manually configure your client.</span></span>
  
## <a name="http-status-errors"></a><span data-ttu-id="6012d-108">Erros de status HTTP</span><span class="sxs-lookup"><span data-stu-id="6012d-108">HTTP status errors</span></span>
<span data-ttu-id="6012d-109"><a name="bk_HttpErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="6012d-109"></span></span>

<span data-ttu-id="6012d-110">O primeiro tipo de erro que você pode encontrar ao enviar solicitações de descoberta automática é o status HTTP.</span><span class="sxs-lookup"><span data-stu-id="6012d-110">The first type of error you might encounter when sending Autodiscover requests is the HTTP status.</span></span> <span data-ttu-id="6012d-111">Se o status HTTP em sua resposta for algo diferente de 200 (Okey), a carga de resposta não contém a resposta da descoberta automática que estava procurando.</span><span class="sxs-lookup"><span data-stu-id="6012d-111">If the HTTP status in your response is anything other than 200 (OK), the response payload doesn't contain the Autodiscover response you were looking for.</span></span> <span data-ttu-id="6012d-112">Para manter a simplicidade, podemos pode agrupar os códigos de status de não-200 em três categorias.</span><span class="sxs-lookup"><span data-stu-id="6012d-112">For simplicity, we can group non-200 status codes into three categories.</span></span>
  
<span data-ttu-id="6012d-113">**Tabela 1. Códigos de status HTTP**</span><span class="sxs-lookup"><span data-stu-id="6012d-113">**Table 1. HTTP status codes**</span></span>

|<span data-ttu-id="6012d-114">**Código de status**</span><span class="sxs-lookup"><span data-stu-id="6012d-114">**Status code**</span></span>|<span data-ttu-id="6012d-115">**Tipo de erro**</span><span class="sxs-lookup"><span data-stu-id="6012d-115">**Type of error**</span></span>|<span data-ttu-id="6012d-116">**Lidar com …**</span><span class="sxs-lookup"><span data-stu-id="6012d-116">**To handle…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6012d-117">301 ou 302</span><span class="sxs-lookup"><span data-stu-id="6012d-117">301 or 302</span></span>  <br/> |<span data-ttu-id="6012d-118">Erro de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="6012d-118">Redirect error</span></span>  <br/> |<span data-ttu-id="6012d-119">Reenvie sua solicitação para o URI contido no cabeçalho da resposta "Local" HTTP.</span><span class="sxs-lookup"><span data-stu-id="6012d-119">Resend your request to the URI contained in the "Location" HTTP response header.</span></span> <span data-ttu-id="6012d-120">Para obter detalhes, consulte [redirecionar de tratamento de erros](#bk_HandlingRedirects).</span><span class="sxs-lookup"><span data-stu-id="6012d-120">For details, see [Handling redirect errors](#bk_HandlingRedirects).</span></span>  <br/> |
|<span data-ttu-id="6012d-121">401</span><span class="sxs-lookup"><span data-stu-id="6012d-121">401</span></span>  <br/> |<span data-ttu-id="6012d-122">Erro não autorizado</span><span class="sxs-lookup"><span data-stu-id="6012d-122">Unauthorized error</span></span>  <br/> |<span data-ttu-id="6012d-123">Porque o [processo de descoberta automática](autodiscover-for-exchange.md) envolve a tentativa de várias URLs possíveis, você poderia obter isso em um URL apenas para ter uma próxima aceitar suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="6012d-123">Because the [Autodiscover process](autodiscover-for-exchange.md) involves trying multiple potential URLs, you could get this on one URL only to have the next one accept your credentials.</span></span> <span data-ttu-id="6012d-124">Por esse motivo, você não deve considerar um erro 401 único para indicar que as credenciais são inválidas.</span><span class="sxs-lookup"><span data-stu-id="6012d-124">For this reason, you shouldn't consider a single 401 error to indicate that the credentials are invalid.</span></span> <span data-ttu-id="6012d-125">No entanto, se você receber 401 erros de várias URLs, você deseja solicitar ao usuário a redigitar sua senha (se possível).</span><span class="sxs-lookup"><span data-stu-id="6012d-125">However, if you receive 401 errors from multiple URLs, you might want to prompt the user to reenter their password (if possible).</span></span>  <br/> |
|<span data-ttu-id="6012d-126">Qualquer outro status de não-200</span><span class="sxs-lookup"><span data-stu-id="6012d-126">Any other non-200 status</span></span>  <br/> |<span data-ttu-id="6012d-127">Erro de ponto de extremidade inválido do descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6012d-127">Invalid Autodiscover endpoint error</span></span>  <br/> |<span data-ttu-id="6012d-128">Considere a URL que retorna qualquer outro código de status de não-200 para ser inválido e continuar a tentar a próxima URL na sua lista.</span><span class="sxs-lookup"><span data-stu-id="6012d-128">Consider the URL that returns any other non-200 status code to be invalid, and continue trying the next URL in your list.</span></span>  <br/> |
   
## <a name="autodiscover-errors"></a><span data-ttu-id="6012d-129">Erros de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6012d-129">Autodiscover errors</span></span>
<span data-ttu-id="6012d-130"><a name="bk_AutodiscoverErrors"> </a></span><span class="sxs-lookup"><span data-stu-id="6012d-130"></span></span>

<span data-ttu-id="6012d-131">Mesmo se você receber um código de status 200 (Okey) após o envio de uma solicitação de descoberta automática, isso não significa que o servidor enviadas as informações que necessárias.</span><span class="sxs-lookup"><span data-stu-id="6012d-131">Even if you get a 200 (OK) status code after sending an Autodiscover request, that doesn't mean that the server sent the information you need.</span></span> <span data-ttu-id="6012d-132">O status de 200 significa apenas que você tenha uma resposta de descoberta automática e essa resposta pode conter um erro dentro da carga.</span><span class="sxs-lookup"><span data-stu-id="6012d-132">The 200 status only means that you have an Autodiscover response, and that response might contain an error within the payload.</span></span> <span data-ttu-id="6012d-133">O local das informações de erro será diferente, dependendo se o formato é SOAP ou POX.</span><span class="sxs-lookup"><span data-stu-id="6012d-133">The location of the error information differs depending on whether the format is SOAP or POX.</span></span>
  
### <a name="soap-autodiscover-errors"></a><span data-ttu-id="6012d-134">Erros de descoberta automática do SOAP</span><span class="sxs-lookup"><span data-stu-id="6012d-134">SOAP Autodiscover errors</span></span>

<span data-ttu-id="6012d-135">Para descoberta automática de SOAP, a resposta pode conter um ou mais elementos [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) , em diferentes locais.</span><span class="sxs-lookup"><span data-stu-id="6012d-135">For SOAP Autodiscover, the response can contain one or more [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) elements, in different places.</span></span> <span data-ttu-id="6012d-136">Normalmente, você pode esperar um como um elemento filho do elemento de [Resposta (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) e outro como um filho do elemento cada [Resposta SOAP ()](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) na resposta.</span><span class="sxs-lookup"><span data-stu-id="6012d-136">Typically you can expect one as a child element of the [Response (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) element, and one as a child of each [UserResponse (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) element in the response.</span></span> <span data-ttu-id="6012d-137">Você também pode encontrar um como um filho do elemento [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , caso haja algum.</span><span class="sxs-lookup"><span data-stu-id="6012d-137">You might also encounter one as a child of a [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) element, if one is present.</span></span> <span data-ttu-id="6012d-138">O contexto do erro depende de onde o elemento **ErrorCode** está localizado, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="6012d-138">The context of the error depends on where the **ErrorCode** element is located, as follows:</span></span> 
  
- <span data-ttu-id="6012d-139">Como um elemento filho do elemento de **resposta** , o elemento **ErrorCode** representa um erro que se aplica a toda a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6012d-139">As a child element of the **Response** element, the **ErrorCode** element represents an error that applies to the entire request.</span></span> 
    
- <span data-ttu-id="6012d-140">Como um filho do elemento de **resposta** , ela representa um erro dizendo que se aplica apenas ao usuário específico.</span><span class="sxs-lookup"><span data-stu-id="6012d-140">As a child of the **UserResponse** element, it represents an error that applies just to that specific user.</span></span> 
    
- <span data-ttu-id="6012d-141">Como um filho de um elemento **UserSettingError** , ela representa um erro que se aplica a uma configuração específica que foi solicitada.</span><span class="sxs-lookup"><span data-stu-id="6012d-141">As a child of a **UserSettingError** element, it represents an error that applies to a specific setting that was requested.</span></span> 
    
<span data-ttu-id="6012d-142">Vamos dar uma olhada em um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6012d-142">Let's take a look at an example of a response.</span></span> <span data-ttu-id="6012d-143">Neste exemplo, o elemento **ErrorCode** sob o elemento de **resposta** tem o valor "NoError", que indica o sucesso geral.</span><span class="sxs-lookup"><span data-stu-id="6012d-143">In this example, the **ErrorCode** element under the **Response** element has a value of "NoError", which indicates overall success.</span></span> <span data-ttu-id="6012d-144">No entanto, o elemento **ErrorCode** sob o elemento de **resposta** tem um valor igual a "RedirectAddress", que indica que ocorreu um erro para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="6012d-144">However, the **ErrorCode** element under the **UserResponse** element has a value of "RedirectAddress", which indicates that an error occurred for that particular user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6012d-145">O artigo [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contém uma lista completa dos erros possíveis.</span><span class="sxs-lookup"><span data-stu-id="6012d-145">The [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) article contains a full list of possible errors.</span></span> <span data-ttu-id="6012d-146">A maioria delas indica um erro irreparável, mas alguns garantem manipulação especial.</span><span class="sxs-lookup"><span data-stu-id="6012d-146">Most of these indicate an unrecoverable error, but a few warrant special handling.</span></span> 
  
<span data-ttu-id="6012d-147">**Tabela 2. Valores de Autodisover ErrorCode SOAP**</span><span class="sxs-lookup"><span data-stu-id="6012d-147">**Table 2. SOAP Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="6012d-148">**Valor ErrorCode**</span><span class="sxs-lookup"><span data-stu-id="6012d-148">**ErrorCode value**</span></span>|<span data-ttu-id="6012d-149">**Lidar com …**</span><span class="sxs-lookup"><span data-stu-id="6012d-149">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6012d-150">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="6012d-150">RedirectAddress</span></span>  <br/> |<span data-ttu-id="6012d-151">[Reiniciando Autodiscover com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6012d-151">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="6012d-152">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="6012d-152">RedirectUrl</span></span>  <br/> |<span data-ttu-id="6012d-153">[Reenvio sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento **RedirectTarget** .</span><span class="sxs-lookup"><span data-stu-id="6012d-153">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the **RedirectTarget** element.</span></span>  <br/> |
|<span data-ttu-id="6012d-154">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="6012d-154">ServerBusy</span></span>  <br/> |<span data-ttu-id="6012d-155">Repita essa URL após um pequeno atraso.</span><span class="sxs-lookup"><span data-stu-id="6012d-155">Retry this URL after a small delay.</span></span> <span data-ttu-id="6012d-156">Você pode esperar um determinado período de tempo ou simplesmente se mudar essa URL ao final da sua lista de URLs para tentar.</span><span class="sxs-lookup"><span data-stu-id="6012d-156">You might wait a set amount of time or simply move this URL to the end of your list of URLs to try.</span></span> <span data-ttu-id="6012d-157">Se você receber esse erro várias vezes, a partir de uma URL, você deve considerar a URL seja inválido.</span><span class="sxs-lookup"><span data-stu-id="6012d-157">If you receive this error multiple times from a URL, you should consider the URL to be invalid.</span></span>  <br/> |
   
### <a name="pox-autodiscover-errors"></a><span data-ttu-id="6012d-158">Erros de descoberta automática POX</span><span class="sxs-lookup"><span data-stu-id="6012d-158">POX Autodiscover errors</span></span>

<span data-ttu-id="6012d-159">O serviço Descoberta automática de POX relata os erros de um pouco diferente.</span><span class="sxs-lookup"><span data-stu-id="6012d-159">The POX Autodiscover service reports errors a little differently.</span></span> <span data-ttu-id="6012d-160">Erros não recuperável estão contidos no elemento [Erro POX ()](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6012d-160">Non-recoverable errors are contained in the [Error (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="6012d-161">O artigo [ErrorCode POX ()](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contém uma lista completa dos códigos de erro possíveis.</span><span class="sxs-lookup"><span data-stu-id="6012d-161">The [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) article contains a full list of possible error codes.</span></span> 
  
<span data-ttu-id="6012d-162">Erros de redirecionamento estão contidos no elemento [Action POX ()](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6012d-162">Redirect errors are contained in the [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="6012d-163">Qualquer valor do elemento **Action** diferente de "configurações" indica um erro de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="6012d-163">Any value of the **Action** element other than "settings" indicates a redirect error.</span></span> 
  
<span data-ttu-id="6012d-164">**Tabela 3. Valores de Autodisover ErrorCode POX**</span><span class="sxs-lookup"><span data-stu-id="6012d-164">**Table 3. POX Autodisover ErrorCode values**</span></span>

|<span data-ttu-id="6012d-165">**Valor de ação**</span><span class="sxs-lookup"><span data-stu-id="6012d-165">**Action value**</span></span>|<span data-ttu-id="6012d-166">**Lidar com …**</span><span class="sxs-lookup"><span data-stu-id="6012d-166">**To handle…**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6012d-167">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="6012d-167">redirectAddr</span></span>  <br/> |<span data-ttu-id="6012d-168">[Reiniciando Autodiscover com um novo endereço de email](#bk_RestartAutodiscover) com o endereço de email no elemento [RedirectAddr POX ()](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6012d-168">[Restarting Autodiscover with a new email address](#bk_RestartAutodiscover) with the email address in the [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) element.</span></span>  <br/> |
|<span data-ttu-id="6012d-169">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="6012d-169">redirectUrl</span></span>  <br/> |<span data-ttu-id="6012d-170">[Reenvio sua solicitação para uma nova URL](#bk_ResendRequest) para a URL no elemento [RedirectUrl POX ()](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6012d-170">[Resending your request to a new URL](#bk_ResendRequest) to the URL in the [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) element.</span></span>  <br/> |
   
<span data-ttu-id="6012d-171">Neste exemplo, o elemento **Action** tem um valor igual a "redirectAddr", que indica que uma nova solicitação deve ser enviada com o novo endereço de email contido no elemento **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="6012d-171">In this example, the **Action** element has a value of "redirectAddr", which indicates that a new request should be sent with the new email address contained in the **RedirectAddr** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a><span data-ttu-id="6012d-172">Tratamento de erros de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="6012d-172">Handling redirect errors</span></span>
<span data-ttu-id="6012d-173"><a name="bk_HandlingRedirects"> </a></span><span class="sxs-lookup"><span data-stu-id="6012d-173"></span></span>

<span data-ttu-id="6012d-174">Você pode manipular os cenários de erro de redirecionamento de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="6012d-174">You can handle redirect error scenarios in two ways:</span></span>
  
- <span data-ttu-id="6012d-175">Reiniciando descoberta automática com um novo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="6012d-175">By restarting Autodiscover with a new email address.</span></span>
    
- <span data-ttu-id="6012d-176">Por reenvio sua solicitação para uma nova URL.</span><span class="sxs-lookup"><span data-stu-id="6012d-176">By resending your request to a new URL.</span></span>
    
<span data-ttu-id="6012d-177">Ambos os cenários exigem alguma validação antes de continuar.</span><span class="sxs-lookup"><span data-stu-id="6012d-177">Both scenarios require some validation before proceeding.</span></span>
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a><span data-ttu-id="6012d-178">Reiniciando descoberta automática com um novo endereço de email</span><span class="sxs-lookup"><span data-stu-id="6012d-178">Restarting Autodiscover with a new email address</span></span>
<span data-ttu-id="6012d-179"><a name="bk_RestartAutodiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="6012d-179"></span></span>

<span data-ttu-id="6012d-180">Quando você obtém um novo endereço de email em uma descoberta automática para redirecionar a resposta, primeiro verifique se o novo endereço de email que foi fornecido na resposta de erro do redirecionamento não é o mesmo endereço que você enviados na solicitação que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="6012d-180">When you get a new email address in an Autodiscover redirect response, first verify that the new email address that was provided in the redirect error response is not the same address that you sent in the request that resulted in the error.</span></span> <span data-ttu-id="6012d-181">Se for, não deve reiniciar a descoberta automática e em vez disso, considere a URL que gerou a resposta para ser inválido.</span><span class="sxs-lookup"><span data-stu-id="6012d-181">If it is, you should not restart Autodiscover and instead consider the URL that generated the response to be invalid.</span></span>
  
<span data-ttu-id="6012d-182">Se o novo endereço de email for diferente, descartar sua lista de possíveis URLs de ponto de extremidade de descoberta automática existentes e gerar uma nova lista com base no novo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="6012d-182">If the new email address is different, discard your existing list of potential Autodiscover endpoint URLs and generate a new list based on the new email address.</span></span>
  
### <a name="resending-your-request-to-a-new-url"></a><span data-ttu-id="6012d-183">Reenvio sua solicitação para uma nova URL</span><span class="sxs-lookup"><span data-stu-id="6012d-183">Resending your request to a new URL</span></span>
<span data-ttu-id="6012d-184"><a name="bk_ResendRequest"> </a></span><span class="sxs-lookup"><span data-stu-id="6012d-184"></span></span>

<span data-ttu-id="6012d-185">Quando você receber uma nova URL em uma resposta de redirecionamento de descoberta automática, você deve primeiro validar a URL da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="6012d-185">When you get a new URL in an Autodiscover redirect response, you should first validate the URL as follows:</span></span>
  
- <span data-ttu-id="6012d-186">Verifique se a URL é uma URL HTTPS.</span><span class="sxs-lookup"><span data-stu-id="6012d-186">Verify that the URL is an HTTPS URL.</span></span>
    
- <span data-ttu-id="6012d-187">Verifique se que você não tiver recebido um erro dessa URL com o endereço de email atual antes.</span><span class="sxs-lookup"><span data-stu-id="6012d-187">Verify that you have not received an error from this URL with the current email address before.</span></span>
    
- <span data-ttu-id="6012d-188">Se aplicável ao seu aplicativo, informar ao usuário sobre o redirecionamento e obtenha sua permissão para seguir o redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="6012d-188">If applicable to your application, inform the user of the redirection and get their permission to follow the redirect.</span></span>
    
- <span data-ttu-id="6012d-189">Envie uma solicitação para a URL e [Verifique se o certificado SSL apresentado pelo servidor é válido](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="6012d-189">Send a request to the URL and [verify that the SSL certificate presented by the server is valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span>
    
<span data-ttu-id="6012d-190">Se a URL passa a validação, reenvie a solicitação para esta nova URL.</span><span class="sxs-lookup"><span data-stu-id="6012d-190">If the URL passes validation, resend the request to this new URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6012d-191">Confira também</span><span class="sxs-lookup"><span data-stu-id="6012d-191">See also</span></span>


- [<span data-ttu-id="6012d-192">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="6012d-192">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="6012d-193">Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange</span><span class="sxs-lookup"><span data-stu-id="6012d-193">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [<span data-ttu-id="6012d-194">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6012d-194">ErrorCode (SOAP)</span></span>](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [<span data-ttu-id="6012d-195">ErrorCode POX)</span><span class="sxs-lookup"><span data-stu-id="6012d-195">ErrorCode (POX)</span></span>](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

