---
title: Obter configurações de usuário do Exchange usando a descoberta automática
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6d90c305-4802-4e18-8d52-f60349feaa8d
description: Saiba como obter definições de configuração do usuário de um servidor do Exchange usando a descoberta automática.
ms.openlocfilehash: f37de55d6681bcdef381561b166adf209d3919a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750724"
---
# <a name="get-user-settings-from-exchange-by-using-autodiscover"></a><span data-ttu-id="0bf82-103">Obter configurações de usuário do Exchange usando a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0bf82-103">Get user settings from Exchange by using Autodiscover</span></span>

<span data-ttu-id="0bf82-104">Saiba como obter definições de configuração do usuário de um servidor do Exchange usando a descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="0bf82-104">Learn how to get user configuration settings from an Exchange server by using Autodiscover.</span></span>
  
<span data-ttu-id="0bf82-105">Descoberta automática simplifica a configuração de aplicativo, fornecendo acesso fácil às informações de configuração do usuário usando apenas o endereço de email do usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="0bf82-105">Autodiscover simplifies application configuration by providing easy access to user configuration information using only the user's email address and password.</span></span> <span data-ttu-id="0bf82-106">Um [número de definições de configuração do usuário](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) estão disponíveis por meio de descoberta automática, como o nome para exibição do usuário ou o URL do serviço web externo.</span><span class="sxs-lookup"><span data-stu-id="0bf82-106">A [number of user configuration settings](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) are available via Autodiscover, such as the user's display name or external web service URL.</span></span> 
  
<span data-ttu-id="0bf82-107">Você pode usar uma das seguintes tecnologias de desenvolvimento para recuperar as configurações de usuário do serviço de descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="0bf82-107">You can use one of the following development technologies to retrieve user settings from the Autodiscover service:</span></span>
  
- <span data-ttu-id="0bf82-108">A [começar com os aplicativos de cliente de API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md)</span><span class="sxs-lookup"><span data-stu-id="0bf82-108">The [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md)</span></span>
    
- <span data-ttu-id="0bf82-109">O [serviço web de descoberta automática do SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0bf82-109">The [SOAP Autodiscover web service](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)</span></span>
    
- <span data-ttu-id="0bf82-110">O [serviço web de descoberta automática de POX](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0bf82-110">The [POX Autodiscover web service](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)</span></span>
    
<span data-ttu-id="0bf82-111">A API gerenciada de EWS fornece uma interface baseada no objeto para recuperar as configurações do usuário.</span><span class="sxs-lookup"><span data-stu-id="0bf82-111">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="0bf82-112">Se seu aplicativo cliente usa código gerenciado, é recomendável que você use a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="0bf82-112">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="0bf82-113">Se você estiver usando a API gerenciada de EWS, determine se as configurações que você precisa estão disponíveis na enumeração [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0bf82-113">If you are using the EWS Managed API, determine whether the settings that you need are available in the [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx) enumeration.</span></span> <span data-ttu-id="0bf82-114">Se eles não forem, convém usar os serviços SOAP ou POX Autodiscover.</span><span class="sxs-lookup"><span data-stu-id="0bf82-114">If they aren't, you might want to use the SOAP or POX Autodiscover services.</span></span> 
  
<span data-ttu-id="0bf82-115">Se você estiver usando um serviço web, sugerimos que você use o serviço de descoberta automática de SOAP, porque ele oferece suporte a um conjunto avançado de recursos do serviço de descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="0bf82-115">If you are using a web service, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span> <span data-ttu-id="0bf82-116">Se o serviço Descoberta automática do SOAP não estiver disponível, o serviço de descoberta automática de POX é uma boa alternativa.</span><span class="sxs-lookup"><span data-stu-id="0bf82-116">If the SOAP Autodiscover service isn't available, the POX Autodiscover service is a good alternative.</span></span>
  
## <a name="set-up-to-get-user-settings"></a><span data-ttu-id="0bf82-117">Configurar o para obter as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="0bf82-117">Set up to get user settings</span></span>
<span data-ttu-id="0bf82-118"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="0bf82-118"></span></span>

<span data-ttu-id="0bf82-119">Antes de você obter configurações de usuário usando o serviço de descoberta automática, certifique-se de que você tenha acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="0bf82-119">Before you get user settings by using the Autodiscover service, make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="0bf82-120">Se você estiver usando o EWS Managed API ou o serviço Descoberta automática de baseados em POX, o Exchange Online, Exchange Online como parte do Office 365 ou um servidor que está executando uma versão do Exchange, começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0bf82-120">If you are using the EWS Managed API or the POX-based Autodiscover service, Exchange Online, Exchange Online as part of Office 365, or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> 
    
- <span data-ttu-id="0bf82-121">Se você estiver usando o serviço de descoberta automática de baseados em SOAP, o Exchange Online ou uma versão do Exchange, começando com o Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="0bf82-121">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
> [!NOTE]
> <span data-ttu-id="0bf82-122">Se você estiver usando a API gerenciada de EWS, você precisará [fornecer um método de retorno de chamada de validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="0bf82-122">If you are using the EWS Managed API, you will need to [provide a certificate validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) in some circumstances.</span></span> <span data-ttu-id="0bf82-123">Talvez você também precise um método de retorno de chamada de validação de certificado com bibliotecas de proxy gerado, como aqueles criados pelo Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="0bf82-123">You might also need a certificate validation callback method with some generated proxy libraries, such as those created by Visual Studio.</span></span> 
  
## <a name="get-user-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="0bf82-124">Obter configurações de usuário usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0bf82-124">Get user settings by using the EWS Managed API</span></span>
<span data-ttu-id="0bf82-125"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="0bf82-125"></span></span>

<span data-ttu-id="0bf82-126">Você pode usar o método [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) para recuperar informações de configuração de um usuário, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="0bf82-126">You can use the [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) method to retrieve configuration information for a user, as shown in the following example.</span></span> <span data-ttu-id="0bf82-127">Neste exemplo, você pode especificar uma matriz de configurações de usuário para retornar (dos que estão disponíveis na enumeração [UserSettingName](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) ) e o método seguirá as respostas de redirecionamento do Exchange server.</span><span class="sxs-lookup"><span data-stu-id="0bf82-127">In this example, you can specify an array of user settings to return (from those available in the [UserSettingName](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx) enumeration), and the method will follow redirection responses from the Exchange server.</span></span> 
  
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

<span data-ttu-id="0bf82-128">Você pode analisar a coleção retornada para acessar cada par de chave/valor na matriz de configurações de usuário.</span><span class="sxs-lookup"><span data-stu-id="0bf82-128">You can parse the collection returned to access each key/value pair in the user settings array.</span></span> <span data-ttu-id="0bf82-129">O exemplo a seguir mostra como fazer o parse por meio de cada elemento retornado e exibir o nome e o valor de cada par de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="0bf82-129">The following example shows how to parse through each returned element and display the name and value of each key/value pair.</span></span>
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
// userresponse is a GetUserSettingsResonse object.
foreach (KeyValuePair<UserSettingName, Object> usersetting in userresponse.Settings)
{
    Console.WriteLine(usersetting.Key.ToString() + ": " + usersetting.Value);
}
```

<span data-ttu-id="0bf82-130">Como alternativa, você pode obter o valor de uma configuração específica.</span><span class="sxs-lookup"><span data-stu-id="0bf82-130">Alternatively, you can obtain the value of a specific setting.</span></span> <span data-ttu-id="0bf82-131">No exemplo a seguir, a configuração de **UserDisplayName** é a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="0bf82-131">In the following example, the **UserDisplayName** setting is to be displayed.</span></span> 
  
```cs
// Display a specific setting, such as UserDisplayName.
Console.WriteLine(userresponse.Settings[UserSettingName.UserDisplayName]);
```

## <a name="get-user-settings-by-using-soap-autodiscover"></a><span data-ttu-id="0bf82-132">Obter configurações de usuário usando a descoberta automática do SOAP</span><span class="sxs-lookup"><span data-stu-id="0bf82-132">Get user settings by using SOAP Autodiscover</span></span>
<span data-ttu-id="0bf82-133"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="0bf82-133"></span></span>

<span data-ttu-id="0bf82-134">Se você não estiver usando o EWS Managed API, recomendamos que você use o serviço web de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="0bf82-134">If you're not using the EWS Managed API, we recommend that you use the SOAP Autodiscover web service.</span></span> <span data-ttu-id="0bf82-135">Use somente o serviço web de descoberta automática de POX se o serviço web de descoberta automática do SOAP falha ou não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0bf82-135">Only use the POX Autodiscover web service if the SOAP Autodiscover web service fails or is not available.</span></span> 
  
<span data-ttu-id="0bf82-136">Para obter as configurações do usuário, use a [operação GetUserSettings (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bf82-136">To get user settings, use the [GetUserSettings operation (SOAP)](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).</span></span> <span data-ttu-id="0bf82-137">As configurações solicitadas são retornadas como [elementos UserSetting](http://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bf82-137">The requested settings are returned as [UserSetting elements](http://msdn.microsoft.com/library/aac6dc31-edd2-49d7-b845-1df4d77da58c%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="0bf82-138">O exemplo a seguir mostra uma solicitação de descoberta automática do SOAP para obter as configurações de usuário do servidor.</span><span class="sxs-lookup"><span data-stu-id="0bf82-138">The following example shows a SOAP Autodiscover request to get user settings from the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="0bf82-139">O exemplo a seguir mostra a resposta SOAP que é retornada pelo servidor após ele analisa a solicitação do cliente.</span><span class="sxs-lookup"><span data-stu-id="0bf82-139">The following example shows the SOAP response that is returned by the server after it parses the request from the client.</span></span> <span data-ttu-id="0bf82-140">A resposta conterá apenas as configurações que são solicitadas, se existirem.</span><span class="sxs-lookup"><span data-stu-id="0bf82-140">The response contains only the settings that are requested, if they exist.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

## <a name="get-user-settings-by-using-pox-autodiscover"></a><span data-ttu-id="0bf82-141">Obter configurações de usuário usando a descoberta automática de POX</span><span class="sxs-lookup"><span data-stu-id="0bf82-141">Get user settings by using POX Autodiscover</span></span>
<span data-ttu-id="0bf82-142"><a name="bk_POX"> </a></span><span class="sxs-lookup"><span data-stu-id="0bf82-142"></span></span>

<span data-ttu-id="0bf82-143">Embora seja recomendável que você use o serviço web de descoberta automática do SOAP, o serviço web de descoberta automática de POX é uma boa opção de backup para esses horários quando SOAP não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0bf82-143">Although we recommend that you use the SOAP Autodiscover web service, the POX Autodiscover web service is a good backup option for those times when SOAP isn't available.</span></span> <span data-ttu-id="0bf82-144">Por exemplo, Exchange 2007 faz não suporte de serviço web SOAP Autodiscover, portanto, se você está direcionando o Exchange 2007, você precisará usar o serviço web de descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="0bf82-144">For example, Exchange 2007 does not support the SOAP Autodiscover web service, so if you are targeting Exchange 2007, you have to use the POX Autodiscover web service.</span></span> <span data-ttu-id="0bf82-145">Diferentemente o serviço web de descoberta automática do SOAP, o serviço Descoberta automática de POX não permite a solicitação de configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="0bf82-145">Unlike the SOAP Autodiscover web service, the POX Autodiscover service does not allow you to request specific settings.</span></span> <span data-ttu-id="0bf82-146">Em vez disso, o servidor retorna uma lista completa de configurações disponíveis como elementos filho do [elemento de protocolo](http://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bf82-146">Instead, the server returns a full list of available settings as child elements of the [Protocol element](http://msdn.microsoft.com/library/f77e4d66-6fdd-4999-9339-f7d7f9c86f44%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="0bf82-147">O exemplo a seguir mostra uma solicitação de descoberta automática de POX para obter as configurações de usuário do servidor.</span><span class="sxs-lookup"><span data-stu-id="0bf82-147">The following example shows a POX Autodiscover request to get user settings from the server.</span></span> <span data-ttu-id="0bf82-148">O XML a seguir é enviado ao servidor por meio de um HTTP POST.</span><span class="sxs-lookup"><span data-stu-id="0bf82-148">The following XML is sent to the server via an HTTP POST.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>mara@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="0bf82-149">O exemplo a seguir mostra a resposta POX retornado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="0bf82-149">The following example shows the POX response that is returned by the server.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
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

## <a name="next-steps"></a><span data-ttu-id="0bf82-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="0bf82-150">Next steps</span></span>
<span data-ttu-id="0bf82-151"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="0bf82-151"></span></span>

<span data-ttu-id="0bf82-152">Depois que você tiver recuperado os detalhes de configuração necessárias para o usuário do servidor, você estará pronto para se comunicar com o Exchange para fazer as coisas que seu aplicativo precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="0bf82-152">After you've retrieved the necessary configuration details for your user from the server, you are ready to communicate with Exchange to do the things your application needs to do.</span></span> <span data-ttu-id="0bf82-153">O que fazer em seguida depende de como você se comunica com o Exchange e o que você deseja realizar.</span><span class="sxs-lookup"><span data-stu-id="0bf82-153">What you do next depends on how you communicate with Exchange and what you want to accomplish.</span></span> <span data-ttu-id="0bf82-154">Se você precisar alguns inspiração, e você estiver usando o EWS, você pode explorar as [amostras de código 101 do Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) para algumas ideias.</span><span class="sxs-lookup"><span data-stu-id="0bf82-154">If you need some inspiration, and you're using EWS, you might explore the [Exchange 101 code samples](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c) for some ideas.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0bf82-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="0bf82-155">See also</span></span>


- [<span data-ttu-id="0bf82-156">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf82-156">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="0bf82-157">API gerenciada de (EWS) de serviços Web do Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf82-157">Exchange Web Services (EWS) Managed API</span></span>](http://msdn.microsoft.com/en-us/library/exchange/jj220535%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="0bf82-158">SOAP referência de serviço web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf82-158">SOAP Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx)
    
- [<span data-ttu-id="0bf82-159">Referência do serviço web POX descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf82-159">POX Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx)
    

