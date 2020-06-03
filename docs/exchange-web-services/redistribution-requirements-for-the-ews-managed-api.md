---
title: Requisitos de redistribuição para a API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Descubra como você pode redistribuir os assemblies da API gerenciada do EWS com seu aplicativo.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463822"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="31e33-103">Requisitos de redistribuição para a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="31e33-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="31e33-104">Descubra como você pode redistribuir os assemblies da API gerenciada do EWS com seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31e33-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="31e33-105">À medida que você projeta seu aplicativo de API gerenciada do EWS, você também deve considerar como você irá liberá-lo para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="31e33-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="31e33-106">Redistribuindo seu aplicativo de API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="31e33-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="31e33-107">A menos que seu aplicativo esteja localizado no servidor Exchange, será necessário redistribuir os assemblies da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="31e33-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="31e33-108">O download da API gerenciada do EWS contém dois assemblies que você pode redistribuir: Microsoft. Exchange. WebServices. dll e Microsoft. Exchange. WebServices. auth. dll.</span><span class="sxs-lookup"><span data-stu-id="31e33-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="31e33-109">Tenha em mente as seguintes informações ao projetar como você vai liberar seu aplicativo de API gerenciada do EWS:</span><span class="sxs-lookup"><span data-stu-id="31e33-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="31e33-110">A API gerenciada do EWS foi projetada para que você possa baixá-lo e distribuí-lo com o aplicativo que tem como alvo um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="31e33-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="31e33-111">Como alternativa, seu aplicativo pode baixar a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="31e33-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="31e33-112">Você pode usar a API gerenciada do EWS para se comunicar com um servidor Exchange executando o Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="31e33-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="31e33-113">Nas versões da API gerenciada do EWS que começam com a versão 2,1, você pode instalar a API no cache de assembly global (GAC).</span><span class="sxs-lookup"><span data-stu-id="31e33-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="31e33-114">O MSI adicionará automaticamente a DLL ao GAC e estará acessível em cada computador, e não em uma base por usuário.</span><span class="sxs-lookup"><span data-stu-id="31e33-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="31e33-115">Os termos de licença estão incluídos no download da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="31e33-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="31e33-116">Revise os termos das informações autoritativas sobre o que você pode fazer com a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="31e33-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="31e33-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="31e33-117">See also</span></span>


- [<span data-ttu-id="31e33-118">Visão geral do design de cliente do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="31e33-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="31e33-119">API gerenciada do EWS (download)</span><span class="sxs-lookup"><span data-stu-id="31e33-119">EWS Managed API (download)</span></span>](https://aka.ms/ews-managed-api-readme)
    

