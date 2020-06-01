---
title: Referência de serviço Web de descoberta automática do SOAP para Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468422"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="18b68-103">Referência de serviço Web de descoberta automática do SOAP para Exchange</span><span class="sxs-lookup"><span data-stu-id="18b68-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="18b68-104">Encontre informações de referência para o serviço de descoberta automática do SOAP no Exchange.</span><span class="sxs-lookup"><span data-stu-id="18b68-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="18b68-105">O serviço de descoberta automática fornece as informações de configuração que o aplicativo usa para criar uma conexão com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="18b68-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="18b68-106">Você pode usar o serviço de descoberta automática do SOAP para enviar mensagens entre o aplicativo cliente e o servidor do Exchange para localizar as configurações que o aplicativo usará para se conectar ao Exchange.</span><span class="sxs-lookup"><span data-stu-id="18b68-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="18b68-107">Ao contrário do serviço de descoberta automática do POX, o serviço de descoberta automática do SOAP permite solicitações de descoberta automática em lote para muitas configurações de usuários e um controle mais granular sobre quais configurações são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="18b68-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="18b68-108">Para clientes que direcionam versões do Exchange a partir do Exchange Server 2010, recomendamos que você use o serviço de descoberta automática do SOAP (em vez do serviço de descoberta automática do POX).</span><span class="sxs-lookup"><span data-stu-id="18b68-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="18b68-109">Os clientes que direcionam o Exchange 2007 precisam usar o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="18b68-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="18b68-110">Recomendamos que os clientes que usam o .NET Framework usem a API gerenciada do EWS, já que contenha um cliente de descoberta automática do SOAP robusto e bem testado.</span><span class="sxs-lookup"><span data-stu-id="18b68-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="18b68-111">Para obter mais informações sobre a API gerenciada do EWS, confira [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="18b68-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="18b68-112">Esta seção fornece informações sobre os elementos XML que são enviados entre o cliente e o servidor durante as redirecionamentos de solicitação de descoberta automática de SOAP e as configurações de usuário retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="18b68-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="18b68-113">A referência do elemento XML contém resumos dos elementos que representam e uma descrição das possíveis hierarquias de elemento que contêm o elemento.</span><span class="sxs-lookup"><span data-stu-id="18b68-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="18b68-114">Os artigos desta seção descrevem as instâncias XML que são enviadas entre o cliente e o servidor.</span><span class="sxs-lookup"><span data-stu-id="18b68-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="18b68-115">O esquema que descreve esses elementos pode ser encontrado no diretório virtual do servidor que hospeda o serviço de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="18b68-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="18b68-116">Os tópicos de operação WSDL nesta seção fornecem uma visão geral do que a operação faz e dos exemplos de resposta e solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="18b68-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="18b68-117">Você pode usar as informações de versão fornecidas para determinar se os recursos que você deseja usar estão disponíveis na versão do produto que você está executando.</span><span class="sxs-lookup"><span data-stu-id="18b68-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="18b68-118">Os exemplos nos tópicos de operação também ajudam a entender a estrutura do XML que está incluída nas mensagens SOAP que são enviadas para e do servidor.</span><span class="sxs-lookup"><span data-stu-id="18b68-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="18b68-119">Esta seção também fornece exemplos e descrições das mensagens usadas para recuperar as informações de configuração da descoberta automática usando o serviço de descoberta automática SOAP.</span><span class="sxs-lookup"><span data-stu-id="18b68-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="18b68-120">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="18b68-120">In this section</span></span>
<span data-ttu-id="18b68-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="18b68-121"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="18b68-122">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18b68-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="18b68-123">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18b68-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="18b68-124">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18b68-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="18b68-125">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18b68-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="18b68-126">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="18b68-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="18b68-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="18b68-127">See also</span></span>


- [<span data-ttu-id="18b68-128">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="18b68-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="18b68-129">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="18b68-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="18b68-130">Usar a Descoberta Automática para localizar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="18b68-130">Use Autodiscover to find connection points</span></span>](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="18b68-131">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="18b68-131">Get user settings from Exchange by using Autodiscover</span></span>](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="18b68-132">Obter as configurações de domínio de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="18b68-132">Get domain settings from an Exchange server</span></span>](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="18b68-133">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="18b68-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

