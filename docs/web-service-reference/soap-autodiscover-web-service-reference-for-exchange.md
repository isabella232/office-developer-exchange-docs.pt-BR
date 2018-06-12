---
title: SOAP referência de serviço web de descoberta automática do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="88eaf-103">SOAP referência de serviço web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="88eaf-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="88eaf-104">Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.</span><span class="sxs-lookup"><span data-stu-id="88eaf-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="88eaf-105">O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão a um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="88eaf-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="88eaf-106">Você pode usar o serviço Descoberta automática do SOAP para enviar mensagens entre o aplicativo cliente e o servidor do Exchange para localizar as configurações que o aplicativo usará para se conectar ao Exchange.</span><span class="sxs-lookup"><span data-stu-id="88eaf-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="88eaf-107">Ao contrário do serviço de descoberta automática de POX, o serviço Descoberta automática do SOAP permite solicitações de descoberta automática em lote para configurações de muitos usuários e controle mais específico sobre quais configurações são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="88eaf-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="88eaf-108">Para clientes que têm como alvo versões do Exchange, começando com o Exchange Server 2010, recomendamos que você use o serviço de descoberta automática de SOAP (em vez do serviço de descoberta automática de POX).</span><span class="sxs-lookup"><span data-stu-id="88eaf-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="88eaf-109">Clientes que visam o Exchange 2007 tem que usar o serviço Descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="88eaf-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="88eaf-110">É recomendável que os clientes que usam o .NET Framework usam a API gerenciada de EWS, porque ele contém um cliente de descoberta automática do SOAP robusto e bem testado.</span><span class="sxs-lookup"><span data-stu-id="88eaf-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="88eaf-111">Para obter mais informações sobre a API gerenciada de EWS, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="88eaf-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="88eaf-112">Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante os redirecionamentos de solicitação de descoberta automática do SOAP e as configurações de usuário que são retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="88eaf-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="88eaf-113">A referência do elemento XML contém resumos dos quais representam os elementos e uma descrição das hierarquias de elemento potenciais que contenham o elemento.</span><span class="sxs-lookup"><span data-stu-id="88eaf-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="88eaf-114">Os artigos nesta seção descrevem as instâncias XML que são enviadas entre o cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="88eaf-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="88eaf-115">O esquema que descreve esses elementos pode ser encontrado no diretório virtual do servidor que hospeda o serviço Descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="88eaf-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="88eaf-116">A operação WSDL tópicos nesta seção fornecem que uma visão geral dos qual a operação e exemplos de solicitação e a resposta de operação.</span><span class="sxs-lookup"><span data-stu-id="88eaf-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="88eaf-117">Você pode usar as informações de versão fornecidas para determinar se os recursos que você deseja usar estão disponíveis no qual você está executando a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="88eaf-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="88eaf-118">Os exemplos nos tópicos a operação também ajudarão-lo a compreender a estrutura do XML que está incluído nas mensagens SOAP que são enviadas para e do servidor.</span><span class="sxs-lookup"><span data-stu-id="88eaf-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="88eaf-119">Esta seção também fornece exemplos e descrições das mensagens que são usadas para recuperar informações de configuração de descoberta automática usando o serviço de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="88eaf-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="88eaf-120">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="88eaf-120">In this section</span></span>
<span data-ttu-id="88eaf-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="88eaf-121"></span></span>

- [<span data-ttu-id="88eaf-122">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88eaf-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="88eaf-123">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88eaf-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="88eaf-124">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88eaf-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="88eaf-125">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88eaf-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="88eaf-126">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="88eaf-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="88eaf-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="88eaf-127">See also</span></span>


- [<span data-ttu-id="88eaf-128">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="88eaf-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="88eaf-129">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="88eaf-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="88eaf-130">Usar descoberta automática para encontrar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="88eaf-130">Use Autodiscover to find connection points</span></span>](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="88eaf-131">Obter configurações de usuário do Exchange usando a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="88eaf-131">Get user settings from Exchange by using Autodiscover</span></span>](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="88eaf-132">Fazer configurações de domínio a partir de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="88eaf-132">Get domain settings from an Exchange server</span></span>](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="88eaf-133">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="88eaf-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

