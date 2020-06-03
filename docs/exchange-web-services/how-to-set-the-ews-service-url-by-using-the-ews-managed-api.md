---
title: Definir a URL do serviço EWS usando a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Encontre informações sobre como definir a URL do serviço do EWS em seu aplicativo de API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456716"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a><span data-ttu-id="d900e-103">Definir a URL do serviço EWS usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d900e-103">Set the EWS service URL by using the EWS Managed API</span></span>

<span data-ttu-id="d900e-104">Encontre informações sobre como definir a URL do serviço do EWS em seu aplicativo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="d900e-104">Find information about how to set the EWS service URL in your EWS Managed API application.</span></span>
  
<span data-ttu-id="d900e-105">A URL do serviço é o endereço que o Exchange usa para se comunicar com os serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="d900e-105">The service URL is the address that Exchange uses to communicate with Exchange Web Services (EWS).</span></span> <span data-ttu-id="d900e-106">Após o aplicativo da API gerenciada do EWS ter esse endereço e ter acesso apropriado para [se comunicar com o EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), ele pode fazer chamadas para a [classe ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d900e-106">After your EWS Managed API application has this address, and has appropriate access to [communicate with EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), it can make calls to the [ExchangeService class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="d900e-107">A URL de serviço de um servidor Exchange local pode ter a aparência a seguir.</span><span class="sxs-lookup"><span data-stu-id="d900e-107">The service URL for an on-premises Exchange server might look like the following.</span></span> 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

<span data-ttu-id="d900e-108">Você pode definir a URL do EWS em seu aplicativo de algumas maneiras.</span><span class="sxs-lookup"><span data-stu-id="d900e-108">You can set the EWS URL in your application in a couple of ways.</span></span> <span data-ttu-id="d900e-109">Recomendamos que você use o [serviço de descoberta automática](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) para obter a URL porque, em uma grande floresta de servidores, a URL poderá ser alterada se a caixa de correio for migrada para outro servidor.</span><span class="sxs-lookup"><span data-stu-id="d900e-109">We recommend that you use the [Autodiscover service](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) to get the URL because in a large forest of servers, the URL can change if the mailbox is migrated to another server.</span></span> <span data-ttu-id="d900e-110">No entanto, como chamar a descoberta automática pode levar algum tempo e reduzir o aplicativo se você precisar fazer várias chamadas em um curto período de tempo, talvez queira armazenar em cache o valor da URL obtido da descoberta automática e definir manualmente a URL do serviço do EWS com esse valor em cache.</span><span class="sxs-lookup"><span data-stu-id="d900e-110">However, because calling Autodiscover can take some time and can slow down your application if you need to make multiple calls in a short period of time, you might want to cache the URL value you get from Autodiscover and manually set the EWS service URL with this cached value.</span></span> <span data-ttu-id="d900e-111">Isso melhorará o desempenho do seu aplicativo; Apenas certifique-se de usar a descoberta automática para atualizar o valor em cache periodicamente, caso o valor mude no servidor.</span><span class="sxs-lookup"><span data-stu-id="d900e-111">This will improve the performance of your application; just make sure that you use Autodiscover to update your cached value periodically in case the value changes on the server.</span></span> 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a><span data-ttu-id="d900e-112">Definir a URL do serviço do EWS usando o serviço de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d900e-112">Set the EWS service URL by using the Autodiscover service</span></span>
<span data-ttu-id="d900e-113"><a name="bk_SetURLusingAutoDiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="d900e-113"><a name="bk_SetURLusingAutoDiscover"> </a></span></span>

<span data-ttu-id="d900e-114">O método [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) usa o endereço de email para definir o ponto de extremidade [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e permite que seu aplicativo use qualquer método incluído nas classes de proxy do **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="d900e-114">The [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method uses the email address to set the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) endpoint and enables your application to use any methods included in the **ExchangeService** proxy classes.</span></span> <span data-ttu-id="d900e-115">O exemplo a seguir mostra como usar o método **AutodiscoverURL** .</span><span class="sxs-lookup"><span data-stu-id="d900e-115">The following example shows how to use the **AutodiscoverURL** method.</span></span> 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a><span data-ttu-id="d900e-116">Definir a URL do serviço do Exchange manualmente</span><span class="sxs-lookup"><span data-stu-id="d900e-116">Set the Exchange service URL manually</span></span>
<span data-ttu-id="d900e-117"><a name="bk_SetURLmanually"> </a></span><span class="sxs-lookup"><span data-stu-id="d900e-117"><a name="bk_SetURLmanually"> </a></span></span>

<span data-ttu-id="d900e-118">O exemplo a seguir mostra como definir a URL do serviço do EWS usando um valor em cache.</span><span class="sxs-lookup"><span data-stu-id="d900e-118">The following example shows you how to set the EWS service URL by using a cached value.</span></span> <span data-ttu-id="d900e-119">Antes de fazer isso, certifique-se de usar o serviço de descoberta automática para obter a URL do EWS.</span><span class="sxs-lookup"><span data-stu-id="d900e-119">Before you do this, make sure to use the Autodiscover service to get the EWS URL.</span></span>
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a><span data-ttu-id="d900e-120">Confira também</span><span class="sxs-lookup"><span data-stu-id="d900e-120">See also</span></span>

- [<span data-ttu-id="d900e-121">Introdução aos aplicativos clientes de API gerenciada por EWS</span><span class="sxs-lookup"><span data-stu-id="d900e-121">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)   
- [<span data-ttu-id="d900e-122">Configurando seu ambiente de desenvolvimento de aplicativos do Exchange</span><span class="sxs-lookup"><span data-stu-id="d900e-122">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="d900e-123">Controlar o acesso ao EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d900e-123">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md) 
- [<span data-ttu-id="d900e-124">Comunicar-se com o EWS usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d900e-124">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [<span data-ttu-id="d900e-125">Usar a Descoberta Automática para localizar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="d900e-125">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    

