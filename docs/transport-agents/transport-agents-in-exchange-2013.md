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
ms.openlocfilehash: 1a28ae79e2a7e338ddd6cb1f6961dd14a980b56e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751029"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="b0adb-103">Agentes de transporte no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0adb-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="b0adb-104">Exchange 2013 fornece uma biblioteca de classes que suportam a extensão do comportamento de transporte do Exchange e habilitar a leitura, gravação e conversão de tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b0adb-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="b0adb-105">Você pode usar essas classes para criar aplicativos de transporte do Exchange que leitura, gravação e processam mensagens no pipeline de transporte.</span><span class="sxs-lookup"><span data-stu-id="b0adb-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="b0adb-106">O que você precisa saber sobre os agentes de transporte</span><span class="sxs-lookup"><span data-stu-id="b0adb-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="b0adb-107">Se você está se perguntando sobre...</span><span class="sxs-lookup"><span data-stu-id="b0adb-107">If you're wondering about…</span></span>|<span data-ttu-id="b0adb-108">Leia isto</span><span class="sxs-lookup"><span data-stu-id="b0adb-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0adb-109">Availability</span><span class="sxs-lookup"><span data-stu-id="b0adb-109">Availability</span></span>  <br/> |<span data-ttu-id="b0adb-110">Agentes de transporte estão disponíveis nas versões do Exchange, começando com o Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="b0adb-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="b0adb-111">Agentes de transporte não são suportados no Office 365 ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b0adb-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="b0adb-112">Remote usage</span><span class="sxs-lookup"><span data-stu-id="b0adb-112">Remote usage</span></span>  <br/> |<span data-ttu-id="b0adb-113">Agentes de transporte executado no servidor Exchange e não têm suporte para uso remoto.</span><span class="sxs-lookup"><span data-stu-id="b0adb-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="b0adb-114">Linguagens com suporte</span><span class="sxs-lookup"><span data-stu-id="b0adb-114">Languages supported</span></span>  <br/> |<span data-ttu-id="b0adb-115">Você pode usar qualquer linguagem do .NET Framework para trabalhar com os agentes de transporte.</span><span class="sxs-lookup"><span data-stu-id="b0adb-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="b0adb-116">Ferramentas de teste e depuração disponíveis</span><span class="sxs-lookup"><span data-stu-id="b0adb-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="b0adb-117">Use versões do Visual Studio, começando com o Visual Studio 2012 para depurar agentes de transporte.</span><span class="sxs-lookup"><span data-stu-id="b0adb-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="b0adb-118">Deployment methods</span><span class="sxs-lookup"><span data-stu-id="b0adb-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="b0adb-119">Você pode instalar aplicativos do agente de transporte usando um script do [Shell de gerenciamento do Exchange](../management/exchange-management-shell.md) .</span><span class="sxs-lookup"><span data-stu-id="b0adb-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="b0adb-120">Nesta se��o</span><span class="sxs-lookup"><span data-stu-id="b0adb-120">In this section</span></span>

- [<span data-ttu-id="b0adb-121">Agente de transporte de novos e atualizados APIs no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="b0adb-122">Transporte amostras de código do agente do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="b0adb-123">Transporte conceitos de agente no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="b0adb-124">Lendo e modificando mensagens no pipeline de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="b0adb-125">Criando os agentes de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="b0adb-126">Referência de agente de transporte do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0adb-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="b0adb-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="b0adb-127">See also</span></span>

- [<span data-ttu-id="b0adb-128">Exchange Online e o desenvolvimento do Exchange</span><span class="sxs-lookup"><span data-stu-id="b0adb-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="b0adb-129">Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0adb-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="b0adb-130">Backup e restauração para o Exchange</span><span class="sxs-lookup"><span data-stu-id="b0adb-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

