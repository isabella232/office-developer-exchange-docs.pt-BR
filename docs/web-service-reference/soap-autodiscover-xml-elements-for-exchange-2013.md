---
title: Elementos de Autodiscover XML SOAP para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.
ms.openlocfilehash: 7201ef33060691df70b63d06b2045e1120b0610f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825517"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="32145-103">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="32145-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="32145-104">Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.</span><span class="sxs-lookup"><span data-stu-id="32145-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="32145-105">A documentação desta seção se baseia nas instâncias de elemento XML de descoberta automática de SOAP que são enviadas entre o cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="32145-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="32145-106">Esta documentação de instância XML baseia-se nos arquivos WSDL e do esquema que estão localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="32145-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="32145-107">Usuários autenticados podem navegar para os arquivos de esquema e WSDL usando uma URL semelhante a um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="32145-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="32145-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — o local do arquivo WSDL.</span><span class="sxs-lookup"><span data-stu-id="32145-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="32145-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — o local do esquema de mensagens.</span><span class="sxs-lookup"><span data-stu-id="32145-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — The location of the messages schema.</span></span>
    
<span data-ttu-id="32145-110">O local dos arquivos de esquema e SOAP WSDL de descoberta automática varia de acordo com a instalação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="32145-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="32145-111">O arquivo de esquema messages.xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e o corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="32145-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="32145-112">Este arquivo fornece um mapa geral dos quais a estrutura XML pode ser para uma interação de mensagem de solicitação-resposta determinado.</span><span class="sxs-lookup"><span data-stu-id="32145-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="32145-113">A estrutura XML real que é enviada entre o cliente e o servidor se baseia nas opções e o contexto no qual ele é usado.</span><span class="sxs-lookup"><span data-stu-id="32145-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="32145-114">Os arquivos de esquema definem o que é possível XML.</span><span class="sxs-lookup"><span data-stu-id="32145-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="32145-115">O real intervalo de XML que será enviada pela conexão baseia-se na qual operação é chamado, as informações solicitadas e as configurações do servidor.</span><span class="sxs-lookup"><span data-stu-id="32145-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="32145-116">Se��es relacionadas</span><span class="sxs-lookup"><span data-stu-id="32145-116">Related sections</span></span>
<span data-ttu-id="32145-117"><a name="bk_RelatedSections"> </a></span><span class="sxs-lookup"><span data-stu-id="32145-117"></span></span>

- [<span data-ttu-id="32145-118">SOAP referência de serviço web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-118">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="32145-119">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-119">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
    
- [<span data-ttu-id="32145-120">Referência de serviço de web mensagens unificada para Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-120">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="32145-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="32145-121">See also</span></span>

- [<span data-ttu-id="32145-122">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="32145-123">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="32145-124">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="32145-124">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

