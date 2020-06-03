---
title: Referência do serviço Web de Unificação de mensagens do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: 83afea8a-c716-41df-9eb2-e1000357afb6
description: Encontre o conteúdo de referência para o serviço da Web de Unificação de mensagens (UM) no Exchange.
ms.openlocfilehash: e4bb63f34650dae8fc28016196c97a6b79e69df0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467372"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="54eac-103">Referência do serviço Web de Unificação de mensagens do Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="54eac-104">Encontre o conteúdo de referência para o serviço da Web de Unificação de mensagens (UM) no Exchange.</span><span class="sxs-lookup"><span data-stu-id="54eac-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="54eac-105">O serviço Web de Unificação de mensagens (UM) fornece um ponto de extensibilidade que permite aos clientes ler e alterar informações sobre as propriedades da UM e solicitar que os itens do repositório de caixa de correio sejam analisados e ditados em um dispositivo de telefonia.</span><span class="sxs-lookup"><span data-stu-id="54eac-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="54eac-106">Esta seção contém informações sobre as operações e os elementos que compõem as mensagens XML para o serviço Web da UM.</span><span class="sxs-lookup"><span data-stu-id="54eac-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="54eac-107">Este conteúdo se aplica à URL de ponto de extremidade de serviço semelhante a https:// \<yourclientaccessserver\> . com/EWS/UM2007Legacy. asmx.</span><span class="sxs-lookup"><span data-stu-id="54eac-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="54eac-108">Você pode usar o serviço de descoberta automática para obter a URL para o ponto de extremidade do serviço Web da UM.</span><span class="sxs-lookup"><span data-stu-id="54eac-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="54eac-109">Para obter mais informações sobre a descoberta automática, confira [descoberta automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="54eac-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="54eac-110">Para as versões do Exchange a partir do Exchange 2010, recomendamos que você use as operações de Unificação de mensagens disponíveis nos [Serviços Web do Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) , em vez do serviço da um, pelos seguintes motivos:</span><span class="sxs-lookup"><span data-stu-id="54eac-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="54eac-111">Os recursos da UM com base no EWS têm suporte de primeira classe na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="54eac-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="54eac-112">Nas versões do Exchange a partir do Exchange 2010, novos recursos da UM são adicionados ao EWS, mas não ao serviço Web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="54eac-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="54eac-113">O serviço Web da UM não tem um esquema explícito.</span><span class="sxs-lookup"><span data-stu-id="54eac-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="54eac-114">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="54eac-114">In this section</span></span>
<span data-ttu-id="54eac-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="54eac-115"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="54eac-116">Operações do serviço Web de Unificação de mensagens para o Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="54eac-117">Elementos XML do serviço Web de Unificação de mensagens para o Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="54eac-118">Confira também</span><span class="sxs-lookup"><span data-stu-id="54eac-118">See also</span></span>

- [<span data-ttu-id="54eac-119">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="54eac-120">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="54eac-121">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="54eac-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

