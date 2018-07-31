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
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353389"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="6e64f-103">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6e64f-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="6e64f-104">Encontre informações de referência de elemento XML para o serviço web de descoberta automática do SOAP no Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e64f-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="6e64f-105">A documentação desta seção se baseia nas instâncias de elemento XML de descoberta automática de SOAP que são enviadas entre o cliente e servidor.</span><span class="sxs-lookup"><span data-stu-id="6e64f-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="6e64f-106">Esta documentação de instância XML baseia-se nos arquivos WSDL e do esquema que estão localizados no diretório virtual que hospeda o serviço de descoberta automática do SOAP.</span><span class="sxs-lookup"><span data-stu-id="6e64f-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="6e64f-107">Usuários autenticados podem navegar para os arquivos de esquema e WSDL usando uma URL semelhante a um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="6e64f-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="6e64f-108">O local do arquivo WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="6e64f-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="6e64f-109">O local do esquema de mensagens: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="6e64f-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="6e64f-110">O local dos arquivos de esquema e SOAP WSDL de descoberta automática varia de acordo com a instalação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e64f-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="6e64f-111">O arquivo de esquema messages.xsd descreve os elementos XML que podem ser enviados em um cabeçalho SOAP de descoberta automática e o corpo SOAP.</span><span class="sxs-lookup"><span data-stu-id="6e64f-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="6e64f-112">Este arquivo fornece um mapa geral dos quais a estrutura XML pode ser para uma interação de mensagem de solicitação-resposta determinado.</span><span class="sxs-lookup"><span data-stu-id="6e64f-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="6e64f-113">A estrutura XML real que é enviada entre o cliente e o servidor se baseia nas opções e o contexto no qual ele é usado.</span><span class="sxs-lookup"><span data-stu-id="6e64f-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="6e64f-114">Os arquivos de esquema definem o que é possível XML.</span><span class="sxs-lookup"><span data-stu-id="6e64f-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="6e64f-115">O real intervalo de XML que será enviada pela conexão baseia-se na qual operação é chamado, as informações solicitadas e as configurações do servidor.</span><span class="sxs-lookup"><span data-stu-id="6e64f-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="6e64f-116">Se��es relacionadas</span><span class="sxs-lookup"><span data-stu-id="6e64f-116">Related sections</span></span>

- [<span data-ttu-id="6e64f-117">SOAP referência de serviço web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="6e64f-118">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="6e64f-119">Referência de serviço de web mensagens unificada para Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="6e64f-120">Confira também</span><span class="sxs-lookup"><span data-stu-id="6e64f-120">See also</span></span>

- [<span data-ttu-id="6e64f-121">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="6e64f-122">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="6e64f-123">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="6e64f-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

