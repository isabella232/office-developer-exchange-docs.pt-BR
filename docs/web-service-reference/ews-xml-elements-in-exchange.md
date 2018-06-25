---
title: Elementos XML do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Encontre informações de referência para o XML EWS elementos no Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752122"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="ce5a9-103">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="ce5a9-104">Encontre informações de referência para o XML EWS elementos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="ce5a9-105">Serviços Web do Exchange (EWS) é um serviço web baseado em SOAP, o que significa que as mensagens de solicitação e resposta que são enviadas entre o cliente e servidor são compostas de elementos XML.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="ce5a9-106">A documentação desta seção baseia-se em instâncias XML que são enviadas entre o cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="ce5a9-107">As instâncias XML são definidas nos arquivos de esquema e WSDL que estão localizados no diretório virtual que hospeda o EWS.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="ce5a9-108">Se você for um usuário autenticado, você pode navegar para os arquivos de esquema e WSDL usando as seguintes URLs, onde \<yourclientaccessserver\> é o nome do seu servidor de acesso para cliente:</span><span class="sxs-lookup"><span data-stu-id="ce5a9-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="ce5a9-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — o local do arquivo WSDL.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="ce5a9-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — o local do esquema de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="ce5a9-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — o local do esquema tipos.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="ce5a9-112">Os arquivos de esquema que descrevem os elementos XML do EWS fornecem um roteiro geral da estrutura XML que seja possível para interações de mensagem de solicitação de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="ce5a9-113">A estrutura XML real que é enviada entre cliente e servidor varia de acordo com a operação que é chamada, as informações solicitadas e as configurações do servidor.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="ce5a9-114">O arquivo WSDL do EWS, services.wsdl, não totalmente acordo com o WSDL padrão porque ele não inclui uma definição de serviço WSDL.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="ce5a9-115">Isso ocorre porque o EWS não foi projetado para ser hospedados em um computador que tenha um endereço predefinido.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="ce5a9-116">Você pode usar o serviço Descoberta automática para obter o endereço do ponto de extremidade EWS.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="ce5a9-117">Alguns geradores de modelo de objeto do cliente analisar o WSDL e podem encontrar uma condição de erro porque o arquivo WSDL não contém uma definição de serviço WSDL.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="ce5a9-118">Se seu gerador de modelo de objeto encontra um erro, você pode inserir um espaço reservado para definição de WSDL do serviço.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="ce5a9-119">Se você estiver usando o .NET Framework para desenvolver seu aplicativo, é recomendável que você use a [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme), em vez de um gerador de modelo de objeto.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="ce5a9-120">A API gerenciada de EWS fornece um modelo de objeto de fácil utilização para manipular a serialização e desserialização do EWS XML.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="ce5a9-121">Para obter mais informações, consulte [Introdução ao aplicativos cliente do EWS Managed API](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce5a9-121">For more information, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="ce5a9-122">O arquivo de esquema messages.xsd contém as definições de elemento para os elementos de nível superior no corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="ce5a9-123">Com exceção dos códigos de resposta de erro, a maioria das definições em messages.xsd é específica para uma operação.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="ce5a9-124">O esquema de types.xsd contém as definições para os cabeçalhos SOAP e todas as definições comuns que são compartilhadas em operações.</span><span class="sxs-lookup"><span data-stu-id="ce5a9-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ce5a9-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="ce5a9-125">See also</span></span>

- [<span data-ttu-id="ce5a9-126">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="ce5a9-127">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="ce5a9-128">Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="ce5a9-129">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="ce5a9-130">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="ce5a9-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

