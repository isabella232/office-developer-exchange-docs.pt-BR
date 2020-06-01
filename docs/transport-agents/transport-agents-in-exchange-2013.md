---
title: Agentes de transporte no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Encontre informações sobre agentes de transporte no Exchange 2013.
ms.openlocfilehash: 62fb259672c47242a57b939deb4887e1e5519e2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461755"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="abe6b-103">Agentes de transporte no Exchange</span><span class="sxs-lookup"><span data-stu-id="abe6b-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="abe6b-104">O Exchange 2013 fornece uma biblioteca de classes que dão suporte à extensão do comportamento de transporte do Exchange e habilitam a leitura, gravação e conversão de tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="abe6b-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="abe6b-105">Você pode usar essas classes para criar aplicativos de transporte do Exchange que lêem, gravam e processam mensagens no pipeline de transporte.</span><span class="sxs-lookup"><span data-stu-id="abe6b-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="abe6b-106">O que você precisa saber sobre agentes de transporte</span><span class="sxs-lookup"><span data-stu-id="abe6b-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="abe6b-107">Se você estiver se perguntando sobre...</span><span class="sxs-lookup"><span data-stu-id="abe6b-107">If you're wondering about…</span></span>|<span data-ttu-id="abe6b-108">Leia isto</span><span class="sxs-lookup"><span data-stu-id="abe6b-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="abe6b-109">Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="abe6b-109">Availability</span></span>  <br/> |<span data-ttu-id="abe6b-110">Os agentes de transporte estão disponíveis em versões do Exchange a partir do Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="abe6b-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="abe6b-111">Os agentes de transporte não têm suporte no Office 365 ou no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="abe6b-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="abe6b-112">Uso remoto</span><span class="sxs-lookup"><span data-stu-id="abe6b-112">Remote usage</span></span>  <br/> |<span data-ttu-id="abe6b-113">Os agentes de transporte são executados no servidor Exchange e não oferecem suporte ao uso remoto.</span><span class="sxs-lookup"><span data-stu-id="abe6b-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="abe6b-114">Linguagens com suporte</span><span class="sxs-lookup"><span data-stu-id="abe6b-114">Languages supported</span></span>  <br/> |<span data-ttu-id="abe6b-115">Você pode usar qualquer linguagem do .NET Framework para trabalhar com agentes de transporte.</span><span class="sxs-lookup"><span data-stu-id="abe6b-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="abe6b-116">Ferramentas de teste e depuração disponíveis</span><span class="sxs-lookup"><span data-stu-id="abe6b-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="abe6b-117">Use versões do Visual Studio começando com o Visual Studio 2012 para depurar agentes de transporte.</span><span class="sxs-lookup"><span data-stu-id="abe6b-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="abe6b-118">Métodos de implantação</span><span class="sxs-lookup"><span data-stu-id="abe6b-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="abe6b-119">Você pode instalar os aplicativos de agente de transporte usando um script do [Shell de gerenciamento do Exchange](../management/exchange-management-shell.md) .</span><span class="sxs-lookup"><span data-stu-id="abe6b-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="abe6b-120">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="abe6b-120">In this section</span></span>

- [<span data-ttu-id="abe6b-121">APIs de agente de transporte novas e atualizadas no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="abe6b-122">Exemplos de código de agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="abe6b-123">Conceitos de agente de transporte no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="abe6b-124">Leitura e modificação de mensagens no pipeline de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="abe6b-125">Criando agentes de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="abe6b-126">Referência do agente de transporte para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="abe6b-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="abe6b-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="abe6b-127">See also</span></span>

- [<span data-ttu-id="abe6b-128">Desenvolvimento do Exchange Online e do Exchange</span><span class="sxs-lookup"><span data-stu-id="abe6b-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="abe6b-129">Explorar os recursos do EWS Managed API, do EWS e dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="abe6b-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="abe6b-130">Backup e restauração para o Exchange</span><span class="sxs-lookup"><span data-stu-id="abe6b-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

