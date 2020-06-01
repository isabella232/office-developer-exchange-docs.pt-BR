---
title: Elementos XML de descoberta automática SOAP para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Encontre informações de referência do elemento XML para o serviço Web de descoberta automática SOAP no Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465181"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="f8759-103">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f8759-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="f8759-104">Encontre informações de referência do elemento XML para o serviço Web de descoberta automática SOAP no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8759-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="f8759-105">A documentação desta seção é baseada nas instâncias de elemento XML de descoberta automática do SOAP que são enviadas entre o cliente e o servidor.</span><span class="sxs-lookup"><span data-stu-id="f8759-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="f8759-106">Esta documentação da instância XML baseia-se nos arquivos WSDL e de esquema localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="f8759-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="f8759-107">Os usuários autenticados podem navegar para os arquivos WSDL e de esquema usando uma URL semelhante a uma das seguintes:</span><span class="sxs-lookup"><span data-stu-id="f8759-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="f8759-108">O local do arquivo WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="f8759-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="f8759-109">O local do esquema de mensagens: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="f8759-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="f8759-110">O local dos arquivos WSDL e do esquema de descoberta automática SOAP varia com base na instalação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8759-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="f8759-111">O arquivo de esquema messages. xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e no corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="f8759-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="f8759-112">Este arquivo fornece um roteiro geral sobre o que a estrutura XML pode ser para uma determinada interação de mensagem de resposta de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8759-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="f8759-113">A estrutura XML real que é enviada entre o cliente e o servidor baseia-se nas opções e no contexto em que é usada.</span><span class="sxs-lookup"><span data-stu-id="f8759-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="f8759-114">Os arquivos de esquema definem o que é possível para o XML.</span><span class="sxs-lookup"><span data-stu-id="f8759-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="f8759-115">O intervalo real de XML enviado pela conexão baseia-se na operação que é chamada, nas informações solicitadas e nas configurações do servidor.</span><span class="sxs-lookup"><span data-stu-id="f8759-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="f8759-116">Seções relacionadas</span><span class="sxs-lookup"><span data-stu-id="f8759-116">Related sections</span></span>

- [<span data-ttu-id="f8759-117">Referência de serviço Web de descoberta automática do SOAP para Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="f8759-118">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="f8759-119">Referência do serviço Web de Unificação de mensagens do Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="f8759-120">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f8759-120">See also</span></span>

- [<span data-ttu-id="f8759-121">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="f8759-122">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="f8759-123">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8759-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

