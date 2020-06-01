---
title: Solicitação de descoberta automática do POX para o Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: A solicitação de descoberta automática contém uma consulta para a configuração de acesso do cliente de um usuário.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461664"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="586b5-103">Solicitação de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="586b5-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="586b5-104">A solicitação de descoberta automática contém uma consulta para a configuração de acesso do cliente de um usuário.</span><span class="sxs-lookup"><span data-stu-id="586b5-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="586b5-105">Exemplo de solicitação de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="586b5-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="586b5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="586b5-106">Description</span></span>

<span data-ttu-id="586b5-107">O exemplo de XML a seguir mostra um corpo de solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="586b5-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="586b5-108">Código</span><span class="sxs-lookup"><span data-stu-id="586b5-108">Code</span></span>

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="586b5-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="586b5-109">Request Headers</span></span>

<span data-ttu-id="586b5-110">Os seguintes cabeçalhos HTTP são opcionais ao enviar solicitações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="586b5-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="586b5-111">**Tabela 1. Cabeçalhos de solicitação HTTP**</span><span class="sxs-lookup"><span data-stu-id="586b5-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="586b5-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="586b5-112">**Header**</span></span>|<span data-ttu-id="586b5-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="586b5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="586b5-114">X-MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="586b5-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="586b5-115">Se presente e definido como "1", indica que o cliente está solicitando informações que podem ser usadas para se conectar ao servidor usando o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="586b5-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="586b5-116">Esse cabeçalho é aplicável aos clientes que implementam o protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="586b5-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="586b5-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="586b5-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="586b5-118">Este cabeçalho contém uma lista delimitada por vírgulas de recursos aos quais o cliente oferece suporte.</span><span class="sxs-lookup"><span data-stu-id="586b5-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="586b5-119">Os valores possíveis são especificados na tabela 2.</span><span class="sxs-lookup"><span data-stu-id="586b5-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="586b5-120">**Tabela 2. Valores de cabeçalho X-ClientCanHandle**</span><span class="sxs-lookup"><span data-stu-id="586b5-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="586b5-121">**Valor X-ClientCanHandle (não diferencia maiúsculas de minúsculas)**</span><span class="sxs-lookup"><span data-stu-id="586b5-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="586b5-122">**Versão mínima do servidor**</span><span class="sxs-lookup"><span data-stu-id="586b5-122">**Minimum server version**</span></span>|<span data-ttu-id="586b5-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="586b5-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="586b5-124">Negocia</span><span class="sxs-lookup"><span data-stu-id="586b5-124">Negotiate</span></span>  <br/> |<span data-ttu-id="586b5-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="586b5-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="586b5-126">Se esse valor estiver presente, o servidor retornará um valor de "Negotiate" no elemento [AuthPackage (POX)](authpackage-pox.md) se o servidor estiver configurado para aceitar a autenticação de negociação.</span><span class="sxs-lookup"><span data-stu-id="586b5-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="586b5-127">Se esse valor não estiver presente, o servidor não retornará um valor de "Negotiate" no elemento **AuthPackage** .</span><span class="sxs-lookup"><span data-stu-id="586b5-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="586b5-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="586b5-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="586b5-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="586b5-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="586b5-130">Se esse valor estiver presente, o servidor retornará um elemento de [protocolo (POX)](protocol-pox.md) com um [tipo (POX)](type-pox.md) definido como "exhttp" se o servidor estiver configurado para aceitar conexões RPC/http.</span><span class="sxs-lookup"><span data-stu-id="586b5-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="586b5-131">Se esse valor não estiver presente, o servidor não retornará um elemento de **protocolo** com um elemento **Type** definido como "exhttp".</span><span class="sxs-lookup"><span data-stu-id="586b5-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="586b5-132">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="586b5-132">Request elements</span></span>

<span data-ttu-id="586b5-133">Os seguintes elementos são usados no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="586b5-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="586b5-134">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="586b5-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="586b5-135">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="586b5-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="586b5-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="586b5-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="586b5-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="586b5-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="586b5-138">O elemento [LegacyDN (POX)](legacydn-pox.md) pode ser usado no lugar do elemento [EMailAddress (POX)](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="586b5-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="586b5-139">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="586b5-139">Version differences</span></span>

<span data-ttu-id="586b5-140">O cabeçalho X-MapiHttpCapability está disponível no Office 365, no Exchange Online e nas versões locais do Exchange a partir do Build 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="586b5-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="586b5-141">O cabeçalho X-ClientCanHandle está disponível no Office 365, no Exchange Online e nas versões locais do Exchange a partir do Build 15.00.0995.014.</span><span class="sxs-lookup"><span data-stu-id="586b5-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="586b5-142">Também consulte</span><span class="sxs-lookup"><span data-stu-id="586b5-142">See also</span></span>



[<span data-ttu-id="586b5-143">Resposta de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="586b5-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="586b5-144">Referência de serviço Web de descoberta automática do POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="586b5-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="586b5-145">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="586b5-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

