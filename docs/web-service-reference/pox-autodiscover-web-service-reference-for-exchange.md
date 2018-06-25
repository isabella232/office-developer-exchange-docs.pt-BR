---
title: Referência do serviço web POX descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Encontre informações de referência para o serviço de descoberta automática de POX no Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="8a23f-103">Referência do serviço web POX descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="8a23f-104">Encontre informações de referência para o serviço de descoberta automática de POX no Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a23f-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="8a23f-105">O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão a um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a23f-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="8a23f-106">Você pode usar o "XML sem formatação antigo" serviço de descoberta automática (POX) para enviar mensagens que consistem apenas das cargas XML, sem qualquer delimitadores envelopes SOAP, para localizar as configurações de um aplicativo cliente deve ter para se conectar ao Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a23f-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8a23f-107">Para clientes que têm como alvo versões do Exchange, começando com o Exchange Server 2010, recomendamos que você usa o serviço de descoberta automática do SOAP em vez do serviço de descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="8a23f-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="8a23f-108">Clientes que visam o Exchange 2007 tem que usar o serviço Descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="8a23f-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="8a23f-109">É recomendável que os clientes que usam o .NET Framework usam a API gerenciada de EWS, porque ele contém um cliente de descoberta automática de POX robusto e bem testado.</span><span class="sxs-lookup"><span data-stu-id="8a23f-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="8a23f-110">Para obter mais informações sobre a API gerenciada de EWS, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8a23f-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="8a23f-111">Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante os redirecionamentos de solicitação de descoberta automática de POX e as configurações de usuário que são retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8a23f-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="8a23f-112">A referência do elemento XML contém resumos dos quais representam os elementos e uma descrição das hierarquias de elemento potenciais que usam o elemento.</span><span class="sxs-lookup"><span data-stu-id="8a23f-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="8a23f-113">Esta documentação aborda as instâncias XML que são enviadas entre o cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="8a23f-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="8a23f-114">O serviço Descoberta automática de POX não tem um esquema explícito.</span><span class="sxs-lookup"><span data-stu-id="8a23f-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="8a23f-115">Os artigos nesta seção fornecem descrições das mensagens que são usadas para recuperar informações de configuração de descoberta automática usando o serviço de descoberta automática de POX e exemplos.</span><span class="sxs-lookup"><span data-stu-id="8a23f-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="8a23f-116">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="8a23f-116">In this section</span></span>
<span data-ttu-id="8a23f-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="8a23f-117"></span></span>

- [<span data-ttu-id="8a23f-118">Solicitação de descoberta automática POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="8a23f-119">Resposta de descoberta automática POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="8a23f-120">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="8a23f-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="8a23f-121">See also</span></span>

- [<span data-ttu-id="8a23f-122">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="8a23f-123">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="8a23f-124">SOAP referência de serviço web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="8a23f-125">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="8a23f-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

