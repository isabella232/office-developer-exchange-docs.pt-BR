---
title: Arquivamento no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Saiba mais sobre o arquivamento no EWS no Exchange.
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456210"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="c1ea8-103">Arquivamento no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1ea8-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="c1ea8-104">Saiba mais sobre o arquivamento no EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="c1ea8-105">Caixas de correio de arquivo morto são caixas de correio secundárias associadas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-105">Archive mailboxes are secondary mailboxes that are associated with a user.</span></span> <span data-ttu-id="c1ea8-106">As caixas de correio de arquivo morto normalmente são usadas para gerenciar limites de armazenamento de email.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-106">Archive mailboxes are typically used to manage email storage limits.</span></span> <span data-ttu-id="c1ea8-107">Por exemplo, os itens de email mais antigos podem ser movidos periodicamente da caixa de entrada para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-107">For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="c1ea8-108">O Exchange Online, o Exchange Online como parte do Office 365 e o Exchange Server 2013 apresentam duas novas operações do EWS (serviços Web do Exchange) que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="c1ea8-109">O arquivamento de itens da caixa de entrada dessa forma preserva a hierarquia de pastas dos itens.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="c1ea8-110">Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente ou remotamente, de modo mais opaco para um usuário, usando um caminho de pasta para apontar para o conteúdo do arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="c1ea8-111">Operações de arquivamento no EWS</span><span class="sxs-lookup"><span data-stu-id="c1ea8-111">Archiving operations in EWS</span></span>

<span data-ttu-id="c1ea8-112">A tabela a seguir lista as operações de arquivamento que foram introduzidas no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="c1ea8-113">**Nome da operação**</span><span class="sxs-lookup"><span data-stu-id="c1ea8-113">**Operation name**</span></span>|<span data-ttu-id="c1ea8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1ea8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1ea8-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="c1ea8-115">ArchiveItem</span></span>](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="c1ea8-116">Move um item da caixa de correio principal para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c1ea8-117">Createfolderpath</span><span class="sxs-lookup"><span data-stu-id="c1ea8-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="c1ea8-118">Cria um URI que aponta para o local de armazenamento da caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="c1ea8-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1ea8-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1ea8-119">See also</span></span>

- [<span data-ttu-id="c1ea8-120">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="c1ea8-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="c1ea8-121">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="c1ea8-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="c1ea8-122">Visão geral do design de cliente do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="c1ea8-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

