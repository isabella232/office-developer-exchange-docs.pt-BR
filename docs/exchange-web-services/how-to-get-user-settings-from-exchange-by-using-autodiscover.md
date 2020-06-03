---
title: Obter as configurações de usuário do Exchange usando a Descoberta Automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 6d90c305-4802-4e18-8d52-f60349feaa8d
description: Saiba como obter as definições de configuração do usuário de um servidor do Exchange usando a descoberta automática.
localization_priority: Priority
ms.openlocfilehash: 5f7ea04e6b04f674d4cb481cf9243d46437d6950
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527996"
---
# <a name="get-user-settings-from-exchange-by-using-autodiscover"></a><span data-ttu-id="53f81-103">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="53f81-103">Get user settings from Exchange by using Autodiscover</span></span>

<span data-ttu-id="53f81-104">Saiba como obter as definições de configuração do usuário de um servidor do Exchange usando a descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="53f81-104">Learn how to get user configuration settings from an Exchange server by using Autodiscover.</span></span>
  
<span data-ttu-id="53f81-105">A descoberta automática simplifica a configuração do aplicativo fornecendo acesso fácil às informações de configuração do usuário usando apenas o endereço de email e a senha do usuário.</span><span class="sxs-lookup"><span data-stu-id="53f81-105">Autodiscover simplifies application configuration by providing easy access to user configuration information using only the user's email address and password.</span></span> <span data-ttu-id="53f81-106">[Várias definições de configuração do usuário](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) estão disponíveis por meio da descoberta automática, como o nome de exibição do usuário ou a URL do serviço Web externo.</span><span class="sxs-lookup"><span data-stu-id="53f81-106">A [number of user configuration settings](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) are available via Autodiscover, such as the user's display name or external web service URL.</span></span> 
  
<span data-ttu-id="53f81-107">Você pode usar uma das seguintes tecnologias de desenvolvimento para recuperar as configurações de usuário do serviço de descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="53f81-107">You can use one of the following development technologies to retrieve user settings from the Autodiscover service:</span></span>
  
- <span data-ttu-id="53f81-108">O [introdução aos aplicativos clientes de API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md)</span><span class="sxs-lookup"><span data-stu-id="53f81-108">The [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md)</span></span>
    
- <span data-ttu-id="53f81-109">O [serviço Web de descoberta automática SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="53f81-109">The [SOAP Autodiscover web service](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span></span>
    
- <span data-ttu-id="53f81-110">O [serviço Web de descoberta automática do Pox](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="53f81-110">The [POX Autodiscover web service](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span></span>
    
<span data-ttu-id="53f81-111">A API gerenciada do EWS fornece uma interface baseada em objeto para recuperar as configurações do usuário.</span><span class="sxs-lookup"><span data-stu-id="53f81-111">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="53f81-112">Se seu aplicativo cliente usa código gerenciado, recomendamos que você use a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="53f81-112">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="53f81-113">Se você estiver usando a API gerenciada do EWS, determine se as configurações de que você precisa estão disponíveis na enumeração [Microsoft. Exchange. WebServices. AutoDiscovery. Usersettingname](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="53f81-113">If you are using the EWS Managed API, determine whether the settings that you need are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span> <span data-ttu-id="53f81-114">Se não forem, talvez você queira usar os serviços de descoberta automática SOAP ou POX.</span><span class="sxs-lookup"><span data-stu-id="53f81-114">If they aren't, you might want to use the SOAP or POX Autodiscover services.</span></span> 
  
<span data-ttu-id="53f81-115">Se você estiver usando um serviço Web, sugerimos que você use o serviço de descoberta automática SOAP, pois ele oferece suporte a um conjunto mais amplo de recursos do que o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="53f81-115">If you are using a web service, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span> <span data-ttu-id="53f81-116">Se o serviço descoberta automática SOAP não estiver disponível, o serviço de descoberta automática do POX será uma boa alternativa.</span><span class="sxs-lookup"><span data-stu-id="53f81-116">If the SOAP Autodiscover service isn't available, the POX Autodiscover service is a good alternative.</span></span>
  
## <a name="set-up-to-get-user-settings"></a><span data-ttu-id="53f81-117">Configurar para obter as configurações do usuário</span><span class="sxs-lookup"><span data-stu-id="53f81-117">Set up to get user settings</span></span>
<span data-ttu-id="53f81-118"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="53f81-118"><a name="bk_Prereq"> </a></span></span>

<span data-ttu-id="53f81-119">Antes de obter as configurações do usuário usando o serviço de descoberta automática, verifique se você tem acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="53f81-119">Before you get user settings by using the Autodiscover service, make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="53f81-120">Se você estiver usando a API gerenciada do EWS ou o serviço de descoberta automática baseado em POX, o Exchange Online, o Exchange Online como parte do Office 365 ou um servidor que esteja executando uma versão do Exchange a partir do Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="53f81-120">If you are using the EWS Managed API or the POX-based Autodiscover service, Exchange Online, Exchange Online as part of Office 365, or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> 
    
- <span data-ttu-id="53f81-121">Se você estiver usando o serviço de descoberta automática baseado em SOAP, o Exchange Online ou uma versão do Exchange a partir do Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="53f81-121">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
> [!NOTE]
> <span data-ttu-id="53f81-122">Se você estiver usando a API gerenciada do EWS, será necessário [fornecer um método de retorno de chamada de validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="53f81-122">If you are using the EWS Managed API, you will need to [provide a certificate validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) in some circumstances.</span></span> <span data-ttu-id="53f81-123">Você também pode precisar de um método de retorno de chamada de validação de certificado com algumas bibliotecas de proxy geradas, como aquelas criadas pelo Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="53f81-123">You might also need a certificate validation callback method with some generated proxy libraries, such as those created by Visual Studio.</span></span> 
  
## <a name="get-user-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="53f81-124">Obter configurações de usuário usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="53f81-124">Get user settings by using the EWS Managed API</span></span>
<span data-ttu-id="53f81-125"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="53f81-125"><a name="bk_Managed"> </a></span></span>

<span data-ttu-id="53f81-126">Você pode usar o método [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) para recuperar as informações de configuração de um usuário, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="53f81-126">You can use the [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method to retrieve configuration information for a user, as shown in the following example.</span></span> <span data-ttu-id="53f81-127">Neste exemplo, você pode especificar uma matriz de configurações de usuário a ser retornada (dentre as disponíveis na enumeração [Usersettingname](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) ) e o método seguirá as respostas de redirecionamento do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="53f81-127">In this example, you can specify an array of user settings to return (from those available in the [UserSettingName](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) enumeration), and the method will follow redirection responses from the Exchange server.</span></span> 
  
```cs
using System;
using System.Net;
using Microsoft.Exchange.WebServices.Autodiscover;
public static GetUserSettingsResponse GetUserSettings(
    AutodiscoverService service,
    string emailAddress,
    int maxHops,
    params UserSettingName[] settings)
{
    Uri url = null;
    GetUserSettingsResponse response = null;
    for (int attempt = 0; attempt < maxHops; attempt++)
    {
        service.Url = url;
        service.EnableScpLookup = (attempt < 2);
        response = service.GetUserSettings(emailAddress, settings);
        if (response.ErrorCode == AutodiscoverErrorCode.RedirectAddress)
        {
            url = new Uri(response.RedirectTarget);
        }
        else if (response.ErrorCode == AutodiscoverErrorCode.RedirectUrl)
        {
            url = new Uri(response.RedirectTarget);
        }
        else
        {
            return response;
        }
    }
    throw new Exception("No suitable Autodiscover endpoint was found.");
}
```

<span data-ttu-id="53f81-128">Você pode analisar a coleção retornada para acessar cada par chave/valor na matriz de configurações do usuário.</span><span class="sxs-lookup"><span data-stu-id="53f81-128">You can parse the collection returned to access each key/value pair in the user settings array.</span></span> <span data-ttu-id="53f81-129">O exemplo a seguir mostra como analisar cada elemento retornado e exibir o nome e o valor de cada par chave/valor.</span><span class="sxs-lookup"><span data-stu-id="53f81-129">The following example shows how to parse through each returned element and display the name and value of each key/value pair.</span></span>
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
// userresponse is a GetUserSettingsResonse object.
foreach (KeyValuePair<UserSettingName, Object> usersetting in userresponse.Settings)
{
    Console.WriteLine(usersetting.Key.ToString() + ": " + usersetting.Value);
}
```

<span data-ttu-id="53f81-130">Como alternativa, você pode obter o valor de uma configuração específica.</span><span class="sxs-lookup"><span data-stu-id="53f81-130">Alternatively, you can obtain the value of a specific setting.</span></span> <span data-ttu-id="53f81-131">No exemplo a seguir, a configuração **UserDisplayName** será exibida.</span><span class="sxs-lookup"><span data-stu-id="53f81-131">In the following example, the **UserDisplayName** setting is to be displayed.</span></span> 
  
```cs
// Display a specific setting, such as UserDisplayName.
Console.WriteLine(userresponse.Settings[UserSettingName.UserDisplayName]);
```

## <a name="get-user-settings-by-using-soap-autodiscover"></a><span data-ttu-id="53f81-132">Obter configurações de usuário usando a descoberta automática SOAP</span><span class="sxs-lookup"><span data-stu-id="53f81-132">Get user settings by using SOAP Autodiscover</span></span>
<span data-ttu-id="53f81-133"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="53f81-133"><a name="bk_SOAP"> </a></span></span>

<span data-ttu-id="53f81-134">Se você não estiver usando a API gerenciada do EWS, recomendamos usar o serviço Web de descoberta automática SOAP.</span><span class="sxs-lookup"><span data-stu-id="53f81-134">If you're not using the EWS Managed API, we recommend that you use the SOAP Autodiscover web service.</span></span> <span data-ttu-id="53f81-135">Só use o serviço Web de descoberta automática do POX se o serviço Web de descoberta automática do SOAP falhar ou não estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="53f81-135">Only use the POX Autodiscover web service if the SOAP Autodiscover web service fails or is not available.</span></span> 
  
<span data-ttu-id="53f81-136">Para obter as configurações do usuário, use a [operação GetUserSettings (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="53f81-136">To get user settings, use the [GetUserSettings operation (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span></span> <span data-ttu-id="53f81-137">As configurações solicitadas são retornadas como [elementos usersetting](https://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="53f81-137">The requested settings are returned as [UserSetting elements](https://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="53f81-138">O exemplo a seguir mostra uma solicitação de descoberta automática do SOAP para obter as configurações de usuário do servidor.</span><span class="sxs-lookup"><span data-stu-id="53f81-138">The following example shows a SOAP Autodiscover request to get user settings from the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>mara@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>PublicFolderServer</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>ExternalMailboxServer</a:Setting>
          <a:Setting>EcpDeliveryReportUrlFragment</a:Setting>
          <a:Setting>EcpPublishingUrlFragment</a:Setting>
          <a:Setting>EcpTextMessagingUrlFragment</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
          <a:Setting>GroupingInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="53f81-139">O exemplo a seguir mostra a resposta SOAP retornada pelo servidor após a análise da solicitação do cliente.</span><span class="sxs-lookup"><span data-stu-id="53f81-139">The following example shows the SOAP response that is returned by the server after it parses the request from the client.</span></span> <span data-ttu-id="53f81-140">A resposta contém apenas as configurações solicitadas, caso existam.</span><span class="sxs-lookup"><span data-stu-id="53f81-140">The response contains only the settings that are requested, if they exist.</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>Mara Whitley</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=mara</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>649d50b8-a1ce-4bac-8ace-2321   e463f701</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>15.01.0160.004</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007, Exchange2007_SP1, Exchange2010, Exchange2010_SP1, Exchange2010_SP2, Exchange2013</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>dc.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=microsoft/ou=Exchange Administrative Group 
                  (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=mail.contoso.com/cn=Contoso Private MDB</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>PublicFolderServer</Name>
                <Value>public.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpDeliveryReportUrlFragment</Name>
                <Value>PersonalSettings/DeliveryReport.aspx?exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpTextMessagingUrlFragment</Name>
                <Value>?p=sms/textmessaging.slab&amp;amp;exsvurl=1</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EcpPublishingUrlFragment</Name>
                <Value>customize/calendarpublishing.slab?exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://mail.contoso.com/EWS/Exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalMailboxServer</Name>
                <Value>mail.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>GroupingInformation</Name>
                <Value>CONTOSO-1</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope
```

## <a name="get-user-settings-by-using-pox-autodiscover"></a><span data-ttu-id="53f81-141">Obter configurações de usuário usando a descoberta automática de POX</span><span class="sxs-lookup"><span data-stu-id="53f81-141">Get user settings by using POX Autodiscover</span></span>
<span data-ttu-id="53f81-142"><a name="bk_POX"> </a></span><span class="sxs-lookup"><span data-stu-id="53f81-142"><a name="bk_POX"> </a></span></span>

<span data-ttu-id="53f81-143">Embora seja recomendável usar o serviço Web de descoberta automática SOAP, o serviço Web de descoberta automática do POX é uma boa opção de backup para os horários em que SOAP não está disponível.</span><span class="sxs-lookup"><span data-stu-id="53f81-143">Although we recommend that you use the SOAP Autodiscover web service, the POX Autodiscover web service is a good backup option for those times when SOAP isn't available.</span></span> <span data-ttu-id="53f81-144">Por exemplo, o Exchange 2007 não é compatível com o serviço Web de descoberta automática do SOAP, portanto, se você estiver direcionando o Exchange 2007, terá que usar o serviço Web de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="53f81-144">For example, Exchange 2007 does not support the SOAP Autodiscover web service, so if you are targeting Exchange 2007, you have to use the POX Autodiscover web service.</span></span> <span data-ttu-id="53f81-145">Diferentemente do serviço Web de descoberta automática do SOAP, o serviço de descoberta automática do POX não permite que você solicite configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="53f81-145">Unlike the SOAP Autodiscover web service, the POX Autodiscover service does not allow you to request specific settings.</span></span> <span data-ttu-id="53f81-146">Em vez disso, o servidor retorna uma lista completa de configurações disponíveis como elementos filhos do [elemento Protocol](https://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="53f81-146">Instead, the server returns a full list of available settings as child elements of the [Protocol element](https://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="53f81-147">O exemplo a seguir mostra uma solicitação de descoberta automática de POX para obter as configurações de usuário do servidor.</span><span class="sxs-lookup"><span data-stu-id="53f81-147">The following example shows a POX Autodiscover request to get user settings from the server.</span></span> <span data-ttu-id="53f81-148">O seguinte XML é enviado ao servidor por meio de um HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="53f81-148">The following XML is sent to the server via an HTTP POST.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>mara@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="53f81-149">O exemplo a seguir mostra a resposta POX retornada pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="53f81-149">The following example shows the POX response that is returned by the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <User>
      <DisplayName>Mara Whitley</DisplayName>
      <LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=f5eeabead90d4b6fb51d6379474692cd-Mara</LegacyDN>
      <AutoDiscoverSMTPAddress>mara@contoso.com</AutoDiscoverSMTPAddress>
      <DeploymentId>50817eff-b925-4578-a0db-13bfc635e7a5</DeploymentId>
    </User>
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <MicrosoftOnline>False</MicrosoftOnline>
      <Protocol>
        <Type>EXCH</Type>
        <Server>5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</Server>
        <ServerDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com</ServerDN>
        <ServerVersion>73C08204</ServerVersion>
        <MdbDN>/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Configuration/cn=Servers/cn=5f76be3c-9138-4f66-85e0-21bc23ca35f0@contoso.com/cn=Microsoft Private MDB</MdbDN>
        <PublicFolderServer>public.contoso.com</PublicFolderServer>
        <AD>dc.contoso.com</AD>
        <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
        <EwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EwsUrl>
        <EmwsUrl>https://mail.contoso.com/EWS/Exchange.asmx</EmwsUrl>
        <EcpUrl>https://mail.contoso.com/ecp/</EcpUrl>
        <EcpUrl-um>?rfr=olk&amp;amp;p=customize/voicemail.aspx&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-um>
        <EcpUrl-aggr>?rfr=olk&amp;amp;p=personalsettings/EmailSubscriptions.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-aggr>
        <EcpUrl-mt>PersonalSettings/DeliveryReport.aspx?rfr=olk&amp;amp;exsvurl=1&amp;amp;IsOWA=&amp;lt;IsOWA&amp;gt;&amp;amp;MsgID=&amp;lt;MsgID&amp;gt;&amp;amp;Mbx=&amp;lt;Mbx&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-mt>
        <EcpUrl-ret>?rfr=olk&amp;amp;p=organize/retentionpolicytags.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-ret>
        <EcpUrl-sms>?rfr=olk&amp;amp;p=sms/textmessaging.slab&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-sms>
        <EcpUrl-publish>customize/calendarpublishing.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;FldID=&amp;lt;FldID&amp;gt;&amp;amp;realm=contoso.com</EcpUrl-publish>
        <EcpUrl-photo>PersonalSettings/EditAccount.aspx?rfr=olk&amp;amp;chgPhoto=1&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-photo>
        <EcpUrl-tm>?rfr=olk&amp;amp;ftr=TeamMailbox&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tm>
        <EcpUrl-tmCreating>?rfr=olk&amp;amp;ftr=TeamMailboxCreating&amp;amp;SPUrl=&amp;lt;SPUrl&amp;gt;&amp;amp;Title=&amp;lt;Title&amp;gt;&amp;amp;SPTMAppUrl=&amp;lt;SPTMAppUrl&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmCreating>
        <EcpUrl-tmEditing>?rfr=olk&amp;amp;ftr=TeamMailboxEditing&amp;amp;Id=&amp;lt;Id&amp;gt;&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-tmEditing>
        <EcpUrl-extinstall>Extension/InstalledExtensions.slab?rfr=olk&amp;amp;exsvurl=1&amp;amp;realm=contoso.com</EcpUrl-extinstall>
        <OOFUrl>https://mail.contoso.com/EWS/Exchange.asmx</OOFUrl>
        <UMUrl>https://mail.contoso.com/EWS/UM2007Legacy.asmx</UMUrl>
        <OABUrl>https://mail.contoso.com/OAB/c21c7bc2-53b3-4ddc-ad89-1219b486c37c/</OABUrl>
        <ServerExclusiveConnect>off</ServerExclusiveConnect>
      </Protocol>
      <Protocol>
        <Type>EXPR</Type>
        <Server>mail.contoso.com</Server>
        <SSL>Off</SSL>
        <AuthPackage>Ntlm</AuthPackage>
        <ServerExclusiveConnect>on</ServerExclusiveConnect>
        <CertPrincipalName>None</CertPrincipalName>
      </Protocol>
      <Protocol>
        <Type>WEB</Type>
        <Internal>
          <OWAUrl AuthenticationMethod="Basic, Fba">https://mail.contoso.com/owa/</OWAUrl>
          <Protocol>
            <Type>EXCH</Type>
            <ASUrl>https://mail.contoso.com/EWS/Exchange.asmx</ASUrl>
          </Protocol>
        </Internal>
      </Protocol>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="next-steps"></a><span data-ttu-id="53f81-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="53f81-150">Next steps</span></span>
<span data-ttu-id="53f81-151"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="53f81-151"><a name="bk_Next"> </a></span></span>

<span data-ttu-id="53f81-152">Depois de recuperar os detalhes de configuração necessários para o usuário do servidor, você está pronto para se comunicar com o Exchange para fazer o que seu aplicativo precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="53f81-152">After you've retrieved the necessary configuration details for your user from the server, you are ready to communicate with Exchange to do the things your application needs to do.</span></span> <span data-ttu-id="53f81-153">O que você faz a seguir depende de como você se comunica com o Exchange e o que você deseja realizar.</span><span class="sxs-lookup"><span data-stu-id="53f81-153">What you do next depends on how you communicate with Exchange and what you want to accomplish.</span></span> <span data-ttu-id="53f81-154">Se você precisar de uma inspiração e estiver usando o EWS, poderá explorar os [exemplos de código do Exchange 101](https://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) para algumas ideias.</span><span class="sxs-lookup"><span data-stu-id="53f81-154">If you need some inspiration, and you're using EWS, you might explore the [Exchange 101 code samples](https://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) for some ideas.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="53f81-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="53f81-155">See also</span></span>


- [<span data-ttu-id="53f81-156">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="53f81-156">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="53f81-157">Serviços Web do Exchange (EWS) Managed API</span><span class="sxs-lookup"><span data-stu-id="53f81-157">Exchange Web Services (EWS) Managed API</span></span>](https://msdn.microsoft.com/library/exchange/jj220535%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="53f81-158">Referência de serviço Web de descoberta automática do SOAP para Exchange</span><span class="sxs-lookup"><span data-stu-id="53f81-158">SOAP Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [<span data-ttu-id="53f81-159">Referência de serviço Web de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="53f81-159">POX Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    

