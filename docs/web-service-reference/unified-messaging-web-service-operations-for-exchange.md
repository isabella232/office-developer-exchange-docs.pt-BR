---
title: Operações do serviço Web de Unificação de mensagens para o Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: d92455bd-24e8-4255-9f93-2bdeff00d42d
description: Encontre informações de referência para as operações do serviço Web de Unificação de mensagens no Exchange.
ms.openlocfilehash: b13ca2fbc44846db0bc98b3961916ba5d0872310
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529711"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="abc8f-103">Operações do serviço Web de Unificação de mensagens para o Exchange</span><span class="sxs-lookup"><span data-stu-id="abc8f-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="abc8f-104">Encontre informações de referência para as operações do serviço Web de Unificação de mensagens no Exchange.</span><span class="sxs-lookup"><span data-stu-id="abc8f-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="abc8f-105">O serviço Web de Unificação de mensagens oferece muitas operações que permitem que os aplicativos cliente leiam e alterem as propriedades de Unificação de mensagens, reproduza mensagens de caixa postal, grave saudações e dite os itens de caixa de correio em dispositivos de telefonia.</span><span class="sxs-lookup"><span data-stu-id="abc8f-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="abc8f-106">Os artigos desta seção fornecem informações sobre a estrutura geral das mensagens de solicitação e resposta para as operações.</span><span class="sxs-lookup"><span data-stu-id="abc8f-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="abc8f-107">Estes artigos fornecem exemplos que mostram estruturas de mensagens comuns.</span><span class="sxs-lookup"><span data-stu-id="abc8f-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="abc8f-108">Você pode usar esses exemplos para saber o que pode fazer com uma solicitação de serviço da Web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="abc8f-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="abc8f-109">Para as versões do Exchange a partir do Exchange 2010, recomendamos que você use as operações de Unificação de mensagens disponíveis nos [Serviços Web do Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) , em vez do serviço Web de Unificação de mensagens, pelos seguintes motivos:</span><span class="sxs-lookup"><span data-stu-id="abc8f-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="abc8f-110">Os recursos de Unificação de mensagens baseados em EWS têm suporte de primeira classe na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="abc8f-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="abc8f-111">Nas versões do Exchange a partir do Exchange 2010, novos recursos de Unificação de mensagens são adicionados ao EWS, mas não ao serviço Web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="abc8f-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="abc8f-112">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="abc8f-112">In this section</span></span>
<span data-ttu-id="abc8f-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="abc8f-113"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="abc8f-114">Operação de desconexão (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="abc8f-115">Operação GetCallInfo (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-116">Operação GetUMProperties (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-117">Operação IsUMEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-118">Operação PlayOnPhone (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-119">Operação PlayOnPhoneGreeting (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-120">Operação ResetPIN (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-121">Operação SetMissedCallNotificationEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="abc8f-122">Operação SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="abc8f-123">Operação SetPlayOnPhoneDialString (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="abc8f-124">Operação SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="abc8f-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="abc8f-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="abc8f-125">See also</span></span>

- [<span data-ttu-id="abc8f-126">Referência do serviço Web de Unificação de mensagens do Exchange</span><span class="sxs-lookup"><span data-stu-id="abc8f-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="abc8f-127">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="abc8f-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="abc8f-128">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="abc8f-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

