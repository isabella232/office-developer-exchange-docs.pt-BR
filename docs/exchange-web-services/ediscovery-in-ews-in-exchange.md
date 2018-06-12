---
title: eDiscovery do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Saiba mais sobre descoberta eletrônica no EWS no Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750649"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="ca00e-103">eDiscovery do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ca00e-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="ca00e-104">Saiba mais sobre descoberta eletrônica no EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca00e-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="ca00e-105">descoberta eletrônica é um serviço web de consulta federados que permite que aplicativos externos executar consultas de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca00e-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="ca00e-106">Descoberta consiste em várias fases, incluindo identificando e preservar dados de chave, remoção para baixo e revisar os dados e produzindo dados no tribunal.</span><span class="sxs-lookup"><span data-stu-id="ca00e-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="ca00e-107">consultas do eDiscovery facilitam o processo de descoberta, fornecendo um fluxo de trabalho de descoberta único entre Exchange e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ca00e-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="ca00e-108">operações de descoberta eletrônica</span><span class="sxs-lookup"><span data-stu-id="ca00e-108">eDiscovery operations</span></span>

<span data-ttu-id="ca00e-109">A funcionalidade de descoberta eletrônica que é exposta por EWS está disponível por meio de operações introduzidas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ca00e-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="ca00e-110">**Tabela 1. Novas operações para a descoberta eletrônica**</span><span class="sxs-lookup"><span data-stu-id="ca00e-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="ca00e-111">**Nome da operação**</span><span class="sxs-lookup"><span data-stu-id="ca00e-111">**Operation name**</span></span>|<span data-ttu-id="ca00e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca00e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca00e-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca00e-113">GetDiscoverySearchConfiguration</span></span>](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-114">Obtém informações de configuração de bloqueio in-loco, salvo pesquisas de descoberta e as caixas de correio que estão habilitadas para pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="ca00e-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="ca00e-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ca00e-115">GetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-116">Obtém o status de uma isenção baseado em consulta, que é definido usando a [operação SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ca00e-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="ca00e-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="ca00e-117">GetNonIndexableItemDetails</span></span>](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-118">Recupera os detalhes sobre os itens que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="ca00e-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="ca00e-119">Isso inclui, mas não está limitado a, o identificador do item, um código de erro, uma descrição do erro, quando foi feita uma tentativa para indexar o item e informações adicionais sobre o arquivo.</span><span class="sxs-lookup"><span data-stu-id="ca00e-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="ca00e-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="ca00e-120">GetNonIndexableItemStatistics</span></span>](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-121">Recupera a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ca00e-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ca00e-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ca00e-122">GetSearchableMailboxes</span></span>](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-123">Obtém uma lista de caixas de correio que o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="ca00e-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="ca00e-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="ca00e-124">SearchMailboxes</span></span>](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-125">Procura por itens em caixas de correio específicas que coincidem com palavras-chave de consulta.</span><span class="sxs-lookup"><span data-stu-id="ca00e-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="ca00e-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ca00e-126">SetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="ca00e-127">Define uma consulta com base em espera em itens.</span><span class="sxs-lookup"><span data-stu-id="ca00e-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca00e-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca00e-128">See also</span></span>

- [<span data-ttu-id="ca00e-129">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="ca00e-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="ca00e-130">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="ca00e-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="ca00e-131">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="ca00e-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

