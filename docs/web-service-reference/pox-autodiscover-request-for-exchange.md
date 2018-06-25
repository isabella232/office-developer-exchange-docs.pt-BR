---
title: Solicitação de descoberta automática POX para Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: A solicitação de descoberta automática contém uma consulta para a configuração de acesso de cliente do usuário.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824865"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="d65a6-103">Solicitação de descoberta automática POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d65a6-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="d65a6-104">A solicitação de descoberta automática contém uma consulta para a configuração de acesso de cliente do usuário.</span><span class="sxs-lookup"><span data-stu-id="d65a6-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="d65a6-105">Exemplo de solicitação de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d65a6-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="d65a6-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d65a6-106">Description</span></span>

<span data-ttu-id="d65a6-107">O exemplo XML a seguir mostra o corpo de uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d65a6-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="d65a6-108">Código</span><span class="sxs-lookup"><span data-stu-id="d65a6-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="d65a6-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d65a6-109">Request Headers</span></span>

<span data-ttu-id="d65a6-110">Os seguintes cabeçalhos HTTP são opcionais ao enviar solicitações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d65a6-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="d65a6-111">**Tabela 1. Cabeçalhos de solicitação HTTP**</span><span class="sxs-lookup"><span data-stu-id="d65a6-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="d65a6-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="d65a6-112">**Header**</span></span>|<span data-ttu-id="d65a6-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d65a6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d65a6-114">X-MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="d65a6-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="d65a6-115">Se presente e definida como "1", indica que o cliente está solicitando informações que podem ser usadas para conectar ao servidor por meio do protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d65a6-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="d65a6-116">Este cabeçalho é aplicável a clientes que implementam o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d65a6-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="d65a6-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="d65a6-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="d65a6-118">Este cabeçalho contém uma lista delimitada por vírgula dos recursos que o cliente oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="d65a6-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="d65a6-119">Os valores possíveis são especificados na tabela 2.</span><span class="sxs-lookup"><span data-stu-id="d65a6-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="d65a6-120">**Tabela 2. Valores de cabeçalho X-ClientCanHandle**</span><span class="sxs-lookup"><span data-stu-id="d65a6-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="d65a6-121">**X-ClientCanHandle valor (diferenciam maiusculas e minúsculas)**</span><span class="sxs-lookup"><span data-stu-id="d65a6-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="d65a6-122">**Versão mínima do servidor**</span><span class="sxs-lookup"><span data-stu-id="d65a6-122">**Minimum server version**</span></span>|<span data-ttu-id="d65a6-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d65a6-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d65a6-124">Negociar</span><span class="sxs-lookup"><span data-stu-id="d65a6-124">Negotiate</span></span>  <br/> |<span data-ttu-id="d65a6-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="d65a6-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="d65a6-126">Se este valor estiver presente, o servidor retornará um valor igual a "Negociar" no elemento [AuthPackage (POX)](authpackage-pox.md) se o servidor está configurado para aceitar a autenticação negociar.</span><span class="sxs-lookup"><span data-stu-id="d65a6-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="d65a6-127">Se este valor não estiver presente, o servidor não retornará um valor igual a "Negociar" no elemento **AuthPackage** .</span><span class="sxs-lookup"><span data-stu-id="d65a6-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="d65a6-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="d65a6-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="d65a6-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="d65a6-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="d65a6-130">Se este valor estiver presente, o servidor retornará um elemento de [Protocolo POX ()](protocol-pox.md) com um elemento de [Tipo POX ()](type-pox.md) definido como "EXHTTP" se o servidor está configurado para aceitar conexões de RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d65a6-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="d65a6-131">Se este valor não estiver presente, o servidor não retornará um elemento de **protocolo** com um elemento de **tipo** definido como "EXHTTP".</span><span class="sxs-lookup"><span data-stu-id="d65a6-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="d65a6-132">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d65a6-132">Request elements</span></span>

<span data-ttu-id="d65a6-133">Os seguintes elementos são usados no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="d65a6-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="d65a6-134">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d65a6-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="d65a6-135">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="d65a6-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="d65a6-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="d65a6-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="d65a6-137">EMailAddress POX)</span><span class="sxs-lookup"><span data-stu-id="d65a6-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="d65a6-138">O elemento [LegacyDN POX ()](legacydn-pox.md) pode ser usado no lugar do elemento [EMailAddress POX ()](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d65a6-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="d65a6-139">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="d65a6-139">Version differences</span></span>

<span data-ttu-id="d65a6-140">O cabeçalho X-MapiHttpCapability está disponível no Office 365, Exchange Online e versões do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1) no local.</span><span class="sxs-lookup"><span data-stu-id="d65a6-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="d65a6-141">O cabeçalho X-ClientCanHandle está disponível no Office 365, Exchange Online e versões do Exchange, começando com o build 15.00.0995.014 no local.</span><span class="sxs-lookup"><span data-stu-id="d65a6-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d65a6-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="d65a6-142">See also</span></span>



[<span data-ttu-id="d65a6-143">Resposta de descoberta automática POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d65a6-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="d65a6-144">Referência do serviço web POX descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="d65a6-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="d65a6-145">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d65a6-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

