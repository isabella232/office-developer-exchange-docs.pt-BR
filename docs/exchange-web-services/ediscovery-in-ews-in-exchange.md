---
title: Descoberta eletrônica no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Saiba mais sobre a descoberta eletrônica no EWS no Exchange.
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456091"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="a56a3-103">Descoberta eletrônica no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a56a3-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="a56a3-104">Saiba mais sobre a descoberta eletrônica no EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="a56a3-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="a56a3-105">a descoberta eletrônica é um serviço Web de consulta federada que permite que aplicativos externos realizem consultas de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a56a3-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="a56a3-106">A descoberta consiste em várias fases, incluindo a identificação e preservação de dados importantes, a remoção e a revisão dos dados e a produção de dados no tribunal.</span><span class="sxs-lookup"><span data-stu-id="a56a3-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="a56a3-107">as consultas de descoberta eletrônica facilitam o processo de descoberta fornecendo um único fluxo de trabalho de descoberta no Exchange e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a56a3-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="a56a3-108">operações de descoberta eletrônica</span><span class="sxs-lookup"><span data-stu-id="a56a3-108">eDiscovery operations</span></span>

<span data-ttu-id="a56a3-109">A funcionalidade de descoberta eletrônica exposta pelo EWS está disponível por meio de operações introduzidas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="a56a3-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="a56a3-110">**Tabela 1. Novas operações para descoberta eletrônica**</span><span class="sxs-lookup"><span data-stu-id="a56a3-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="a56a3-111">**Nome da operação**</span><span class="sxs-lookup"><span data-stu-id="a56a3-111">**Operation name**</span></span>|<span data-ttu-id="a56a3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a56a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a56a3-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a56a3-113">GetDiscoverySearchConfiguration</span></span>](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-114">Obtém informações de configuração para bloqueios in-loco, pesquisas salvas de descoberta e caixas de correio habilitadas para pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="a56a3-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="a56a3-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a56a3-115">GetHoldOnMailboxes</span></span>](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-116">Obtém o status de um bloqueio baseado em consulta, que é definido usando a [operação SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a56a3-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="a56a3-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="a56a3-117">GetNonIndexableItemDetails</span></span>](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-118">Recupera os detalhes sobre os itens que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="a56a3-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="a56a3-119">Isso inclui, mas não está limitado a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa é feita para indexar o item e informações adicionais sobre o arquivo.</span><span class="sxs-lookup"><span data-stu-id="a56a3-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="a56a3-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="a56a3-120">GetNonIndexableItemStatistics</span></span>](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-121">Recupera a contagem de itens que não podem ser indexados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a56a3-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a56a3-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="a56a3-122">GetSearchableMailboxes</span></span>](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-123">Obtém uma lista de caixas de correio nas quais o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="a56a3-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="a56a3-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="a56a3-124">SearchMailboxes</span></span>](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-125">Procura itens em caixas de correio específicas que correspondam a palavras-chave de consulta.</span><span class="sxs-lookup"><span data-stu-id="a56a3-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="a56a3-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a56a3-126">SetHoldOnMailboxes</span></span>](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="a56a3-127">Define um bloqueio baseado em consulta nos itens.</span><span class="sxs-lookup"><span data-stu-id="a56a3-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a56a3-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="a56a3-128">See also</span></span>

- [<span data-ttu-id="a56a3-129">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="a56a3-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="a56a3-130">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="a56a3-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="a56a3-131">Visão geral do design de cliente do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="a56a3-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

