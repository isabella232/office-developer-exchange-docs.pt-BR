---
title: Arquivamento no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Saiba mais sobre o arquivamento no EWS no Exchange.
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750639"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="44f4e-103">Arquivamento no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="44f4e-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="44f4e-104">Saiba mais sobre o arquivamento no EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="44f4e-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="44f4e-105">Caixas de correio de arquivo morto são secundárias caixas de correio que estão associadas um usuário.</span><span class="sxs-lookup"><span data-stu-id="44f4e-105">Archive mailboxes are secondary mailboxes that are associated with a user.</span></span> <span data-ttu-id="44f4e-106">Caixas de correio de arquivo morto são geralmente usadas para gerenciar os limites de armazenamento de email.</span><span class="sxs-lookup"><span data-stu-id="44f4e-106">Archive mailboxes are typically used to manage email storage limits.</span></span> <span data-ttu-id="44f4e-107">Por exemplo, itens de email mais antigos periodicamente talvez seja movidos de caixa de entrada para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="44f4e-107">For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="44f4e-108">O Exchange Online, Exchange Online como parte do Office 365 e Exchange Server 2013 introduz duas novas operações de serviços Web do Exchange (EWS) que você pode usar para arquivar um conjunto de itens de email de uma caixa de correio principal.</span><span class="sxs-lookup"><span data-stu-id="44f4e-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="44f4e-109">Arquivamento de itens de caixa de entrada dessa maneira preserva a hierarquia de pastas dos itens.</span><span class="sxs-lookup"><span data-stu-id="44f4e-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="44f4e-110">Além disso, as caixas de correio de arquivo morto agora podem ser armazenadas localmente em um cliente, ou remotamente, de forma que é opaca a um usuário, principalmente por meio de um caminho de pasta para apontar para o conteúdo do arquivamento.</span><span class="sxs-lookup"><span data-stu-id="44f4e-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="44f4e-111">Operações de arquivamento no EWS</span><span class="sxs-lookup"><span data-stu-id="44f4e-111">Archiving operations in EWS</span></span>

<span data-ttu-id="44f4e-112">A tabela a seguir lista as operações de arquivamento que foram introduzidas no Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="44f4e-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="44f4e-113">**Nome da operação**</span><span class="sxs-lookup"><span data-stu-id="44f4e-113">**Operation name**</span></span>|<span data-ttu-id="44f4e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="44f4e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44f4e-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="44f4e-115">ArchiveItem</span></span>](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="44f4e-116">Move um item da caixa de correio principal para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="44f4e-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="44f4e-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="44f4e-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="44f4e-118">Cria um URI que aponta para o local de armazenamento para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="44f4e-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44f4e-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="44f4e-119">See also</span></span>

- [<span data-ttu-id="44f4e-120">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="44f4e-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="44f4e-121">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="44f4e-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="44f4e-122">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="44f4e-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

