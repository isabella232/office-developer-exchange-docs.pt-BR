---
title: Elementos XML do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Encontre informações de referência para os elementos XML do EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526113"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="3e883-103">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="3e883-104">Encontre informações de referência para os elementos XML do EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e883-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="3e883-105">O EWS (serviços Web do Exchange) é um serviço Web baseado em SOAP, o que significa que as mensagens de solicitação e resposta enviadas entre o cliente e o servidor são compostas de elementos XML.</span><span class="sxs-lookup"><span data-stu-id="3e883-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="3e883-106">A documentação desta seção é baseada nas instâncias XML que são enviadas entre o cliente e o servidor.</span><span class="sxs-lookup"><span data-stu-id="3e883-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="3e883-107">As instâncias XML são definidas nos arquivos WSDL e de esquema que estão localizados no diretório virtual que hospeda o EWS.</span><span class="sxs-lookup"><span data-stu-id="3e883-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="3e883-108">Se você for um usuário autenticado, poderá navegar até os arquivos WSDL e de esquema usando as seguintes URLs, onde \<yourclientaccessserver\> é o nome do servidor de acesso para cliente:</span><span class="sxs-lookup"><span data-stu-id="3e883-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="3e883-109">http:// \<yourclientaccessserver\> . com/EWS/Services. WSDL — o local do arquivo WSDL.</span><span class="sxs-lookup"><span data-stu-id="3e883-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="3e883-110">http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — o local do esquema de mensagens.</span><span class="sxs-lookup"><span data-stu-id="3e883-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="3e883-111">http:// \<yourclientaccessserver\> . com/EWS/Types. xsd — o local do esquema de tipos.</span><span class="sxs-lookup"><span data-stu-id="3e883-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="3e883-112">Os arquivos de esquema que descrevem os elementos XML do EWS fornecem um roteiro geral da estrutura XML que é possível para interações de mensagens de resposta de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e883-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="3e883-113">A estrutura XML real que é enviada entre o cliente e o servidor varia de acordo com a operação que é chamada, as informações solicitadas e as configurações do lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="3e883-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="3e883-114">O arquivo WSDL do EWS, Services. WSDL, não está totalmente em conformidade com o padrão WSDL porque não inclui uma definição de serviço WSDL.</span><span class="sxs-lookup"><span data-stu-id="3e883-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="3e883-115">Isso ocorre porque o EWS não foi projetado para ser hospedado em um computador que tenha um endereço predefinido.</span><span class="sxs-lookup"><span data-stu-id="3e883-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="3e883-116">Você pode usar o serviço de descoberta automática para obter o endereço do ponto de extremidade do EWS.</span><span class="sxs-lookup"><span data-stu-id="3e883-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="3e883-117">Alguns geradores de modelos de objeto do lado do cliente analisam o WSDL e podem encontrar uma condição de erro porque o arquivo WSDL não contém uma definição de serviço WSDL.</span><span class="sxs-lookup"><span data-stu-id="3e883-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="3e883-118">Se o gerador do modelo de objeto encontrar um erro, você pode inserir uma definição de serviço WSDL de espaço reservado.</span><span class="sxs-lookup"><span data-stu-id="3e883-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="3e883-119">Se você estiver usando o .NET Framework para desenvolver seu aplicativo, recomendamos que você use a [API gerenciada do EWS](http://aka.ms/ews-managed-api-readme), em vez de um gerador de modelos de objeto.</span><span class="sxs-lookup"><span data-stu-id="3e883-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="3e883-120">A API gerenciada do EWS fornece um modelo de objeto fácil de usar para lidar com a serialização e a desserialização do EWS XML.</span><span class="sxs-lookup"><span data-stu-id="3e883-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="3e883-121">Para obter mais informações, consulte [introdução aos aplicativos clientes de API gerenciada do EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3e883-121">For more information, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="3e883-122">O arquivo de esquema messages. xsd contém as definições de elemento para os elementos de nível superior no corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="3e883-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="3e883-123">Com exceção dos códigos de resposta de erro, a maioria das definições em messages. xsd são específicas para uma operação.</span><span class="sxs-lookup"><span data-stu-id="3e883-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="3e883-124">O esquema Types. xsd contém as definições dos cabeçalhos SOAP e todas as definições comuns que são compartilhadas entre as operações.</span><span class="sxs-lookup"><span data-stu-id="3e883-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="3e883-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="3e883-125">See also</span></span>

- [<span data-ttu-id="3e883-126">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="3e883-127">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="3e883-128">Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="3e883-129">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="3e883-130">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="3e883-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

