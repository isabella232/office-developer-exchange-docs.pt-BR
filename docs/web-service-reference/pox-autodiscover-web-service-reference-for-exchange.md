---
title: Referência de serviço Web de descoberta automática do POX para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Encontre informações de referência para o serviço de descoberta automática do POX no Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465650"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="34e41-103">Referência de serviço Web de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="34e41-104">Encontre informações de referência para o serviço de descoberta automática do POX no Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e41-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="34e41-105">O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e41-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="34e41-106">Você pode usar o serviço de descoberta automática de "Plain Old XML" (POX) para enviar mensagens que consistam apenas de cargas XML, sem nenhum envelope SOAP delimitador, para localizar as configurações que um aplicativo cliente deve ter para se conectar ao Exchange.</span><span class="sxs-lookup"><span data-stu-id="34e41-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="34e41-107">Para clientes que direcionam versões do Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço de descoberta automática SOAP em vez do serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="34e41-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="34e41-108">Os clientes que direcionam o Exchange 2007 precisam usar o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="34e41-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="34e41-109">Recomendamos que os clientes que usam o .NET Framework usem a API gerenciada do EWS, pois ele contém um cliente de descoberta automática do POX e bem testado.</span><span class="sxs-lookup"><span data-stu-id="34e41-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="34e41-110">Para obter mais informações sobre a API gerenciada do EWS, confira [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="34e41-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="34e41-111">Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante o redirecionamento da solicitação de descoberta automática de POX e as configurações de usuário retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="34e41-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="34e41-112">A referência do elemento XML contém resumos dos elementos que representam e uma descrição das possíveis hierarquias de elemento que usam o elemento.</span><span class="sxs-lookup"><span data-stu-id="34e41-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="34e41-113">Esta documentação abrange as instâncias XML que são enviadas entre o cliente e o servidor.</span><span class="sxs-lookup"><span data-stu-id="34e41-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="34e41-114">O serviço de descoberta automática do POX não tem um esquema explícito.</span><span class="sxs-lookup"><span data-stu-id="34e41-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="34e41-115">Os artigos desta seção fornecem exemplos e descrições das mensagens usadas para recuperar as informações de configuração da descoberta automática usando o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="34e41-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="34e41-116">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="34e41-116">In this section</span></span>
<span data-ttu-id="34e41-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="34e41-117"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="34e41-118">Solicitação de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="34e41-119">Resposta de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="34e41-120">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="34e41-121">Também consulte</span><span class="sxs-lookup"><span data-stu-id="34e41-121">See also</span></span>

- [<span data-ttu-id="34e41-122">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="34e41-123">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="34e41-124">Referência de serviço Web de descoberta automática do SOAP para Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="34e41-125">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="34e41-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

