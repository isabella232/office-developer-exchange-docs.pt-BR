---
title: Referência do serviço Web de descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Encontre o conteúdo de referência para o serviço Web de descoberta automática no Exchange.
ms.openlocfilehash: ce7f2bbd662a5e61959c7e3c6748f0cf40cc4fb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466868"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="95e3b-103">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="95e3b-103">Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="95e3b-104">Encontre o conteúdo de referência para o serviço Web de descoberta automática no Exchange.</span><span class="sxs-lookup"><span data-stu-id="95e3b-104">Find reference content for the Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="95e3b-105">O serviço Web de descoberta automática fornece as informações de configuração que seu aplicativo usa para criar uma conexão com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="95e3b-105">The Autodiscover web service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="95e3b-106">Você pode usar uma das seguintes opções para se conectar à descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="95e3b-106">You can use one of the following options to connect to Autodiscover:</span></span>
  
- <span data-ttu-id="95e3b-107">Serviço de descoberta automática SOAP — disponível para clientes que se conectam a versões do Exchange a partir do Exchange 2010, incluindo o Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="95e3b-107">SOAP Autodiscover service —Available to clients that connect to versions of Exchange starting with Exchange 2010, including Exchange Online.</span></span>
    
- <span data-ttu-id="95e3b-108">o serviço de descoberta automática "(" Plain Old XML "), disponível para clientes que se conectam às versões do Exchange a partir do Exchange 2007, incluindo o Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="95e3b-108">"plain old XML" (POX) Autodiscover service — Available to clients that connect to versions of Exchange starting with Exchange 2007, including Exchange Online.</span></span> 
    
<span data-ttu-id="95e3b-109">O serviço descoberta automática SOAP e POX pode fornecer as informações de configuração que seu cliente usará para criar uma conexão com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="95e3b-109">Both the SOAP and the POX Autodiscover service can provide the configuration information that your client will use to create a connection to an Exchange server.</span></span>
  
> [!NOTE]
> <span data-ttu-id="95e3b-110">Para versões do Exchange a partir do Exchange 2010, recomendamos que você use o serviço de descoberta automática do SOAP em vez do serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="95e3b-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="95e3b-111">O serviço de descoberta automática do SOAP fornece solicitações de configuração de descoberta automática em lote e controle mais granular sobre quais configurações são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="95e3b-111">The SOAP Autodiscover service provides batched Autodiscover setting requests and more granular control over which settings are returned in the response.</span></span> 
  
<span data-ttu-id="95e3b-112">Esta seção contém informações de referência para o serviço de descoberta automática do SOAP e o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="95e3b-112">This section contains reference information for the SOAP Autodiscover service and the POX Autodiscover service.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="95e3b-113">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="95e3b-113">In this section</span></span>
<span data-ttu-id="95e3b-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="95e3b-114"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="95e3b-115">Referência de serviço Web de descoberta automática do SOAP para Exchange</span><span class="sxs-lookup"><span data-stu-id="95e3b-115">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="95e3b-116">Referência de serviço Web de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="95e3b-116">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="95e3b-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="95e3b-117">See also</span></span>

- [<span data-ttu-id="95e3b-118">Referência de serviço Web do Exchange</span><span class="sxs-lookup"><span data-stu-id="95e3b-118">Web services reference for Exchange</span></span>](web-services-reference-for-exchange.md)
- [<span data-ttu-id="95e3b-119">Serviço de descoberta automática (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95e3b-119">Autodiscover Service (SOAP)</span></span>](https://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [<span data-ttu-id="95e3b-120">Serviço de descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="95e3b-120">Autodiscover Service (POX)</span></span>](https://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    

