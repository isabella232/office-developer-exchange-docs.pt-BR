---
title: Referência de serviço de web mensagens unificada para Exchange
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
description: Encontre conteúdo de referência para o serviço web de Unificação de mensagens (UM) do Exchange.
ms.openlocfilehash: 12ee91c5a8b7e1ba23b937f142a9ae2835697fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837828"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="dd9c2-103">Referência de serviço de web mensagens unificada para Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="dd9c2-104">Encontre conteúdo de referência para o serviço web de Unificação de mensagens (UM) do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="dd9c2-105">O serviço web de Unificação de mensagens (UM) fornece um ponto de extensibilidade que permite que os clientes ler e alterar as informações sobre as propriedades de Unificação de mensagens e solicitar que os itens do repositório de caixa de correio ser analisados e ditadas por um dispositivo de telefonia.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="dd9c2-106">Esta seção contém informações sobre as operações e os elementos que compõem as mensagens XML para o serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="dd9c2-107">Este conteúdo se aplica para a URL do ponto de extremidade de serviço similar à https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="dd9c2-108">Você pode usar o serviço Descoberta automática para obter a URL do ponto de extremidade do serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="dd9c2-109">Para obter mais informações sobre a descoberta automática, consulte [descoberta automática do Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="dd9c2-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="dd9c2-110">Para versões do Exchange, começando com o Exchange 2010, recomendamos que você use as operações de Unificação de mensagens que estão disponíveis no [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) em vez do serviço web de Unificação de mensagens, pelos seguintes motivos: > recursos de Unificação de mensagens com base no EWS têm suporte de primeira classe na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons: >  The EWS-based UM features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="dd9c2-111">> Nas versões do Exchange, começando com o Exchange 2010, novos recursos de Unificação de mensagens são adicionados ao EWS, mas não para o serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-111">>  In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="dd9c2-112">O serviço web de Unificação de mensagens não tem um esquema explícito.</span><span class="sxs-lookup"><span data-stu-id="dd9c2-112">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="dd9c2-113">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="dd9c2-113">In this section</span></span>
<span data-ttu-id="dd9c2-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="dd9c2-114"></span></span>

- [<span data-ttu-id="dd9c2-115">Operações de serviço de web mensagens unificadas para Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-115">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)
    
- [<span data-ttu-id="dd9c2-116">Unified Messaging web service os elementos XML para o Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="dd9c2-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="dd9c2-117">See also</span></span>

- [<span data-ttu-id="dd9c2-118">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-118">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="dd9c2-119">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-119">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="dd9c2-120">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="dd9c2-120">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

