---
title: Requisitos de redistribuição para a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Descubra como você pode redistribuir os assemblies de API gerenciada de EWS com seu aplicativo.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750946"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="0cf46-103">Requisitos de redistribuição para a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0cf46-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="0cf46-104">Descubra como você pode redistribuir os assemblies de API gerenciada de EWS com seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0cf46-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="0cf46-105">Como criar seu aplicativo EWS Managed API, também desejará considerar como você irá liberá-la para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="0cf46-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="0cf46-106">Redistribuir seu aplicativo API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="0cf46-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="0cf46-107">A menos que o aplicativo está localizado no servidor do Exchange, você precisará redistribuir os assemblies de API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="0cf46-107">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies.</span></span> <span data-ttu-id="0cf46-108">O download do EWS Managed API contém dois assemblies que você pode redistribuir: Microsoft.Exchange.WebServices.dll e Microsoft.Exchange.WebServices.Auth.dll.</span><span class="sxs-lookup"><span data-stu-id="0cf46-108">The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll.</span></span> <span data-ttu-id="0cf46-109">Lembre-se das seguintes informações ao criar como lançará seu aplicativo API gerenciada de EWS:</span><span class="sxs-lookup"><span data-stu-id="0cf46-109">Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="0cf46-110">A API gerenciada de EWS foi projetada, de forma que você pode baixá-lo e distribuí-lo com o seu aplicativo que tem como destino um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cf46-110">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server.</span></span> <span data-ttu-id="0cf46-111">Como alternativa, seu aplicativo pode baixar o EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="0cf46-111">Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="0cf46-112">Você pode usar a API gerenciada de EWS para se comunicar com um servidor do Exchange executando o Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="0cf46-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="0cf46-113">Nas versões do EWS Managed API começando com a versão 2.1, você pode instalar a API no Cache de Assembly Global (GAC).</span><span class="sxs-lookup"><span data-stu-id="0cf46-113">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC).</span></span> <span data-ttu-id="0cf46-114">O MSI adicionará automaticamente a DLL no GAC e será acessível no computador por computador, não em uma base por usuário.</span><span class="sxs-lookup"><span data-stu-id="0cf46-114">The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="0cf46-115">Os termos de licença são incluídos no download do EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="0cf46-115">The license terms are included in the EWS Managed API download.</span></span> <span data-ttu-id="0cf46-116">Analise os termos para obter as informações autoritativas sobre o que você pode fazer com a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="0cf46-116">Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0cf46-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="0cf46-117">See also</span></span>


- [<span data-ttu-id="0cf46-118">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="0cf46-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="0cf46-119">API gerenciada de EWS (download)</span><span class="sxs-lookup"><span data-stu-id="0cf46-119">EWS Managed API (download)</span></span>](http://aka.ms/ews-managed-api-readme)
    

