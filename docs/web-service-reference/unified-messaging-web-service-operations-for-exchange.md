---
title: Operações de serviço de web mensagens unificadas para Exchange
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
description: Encontre informações de referência para as operações de serviço web de Unificação de mensagens no Exchange.
ms.openlocfilehash: 21d3469d752ff6cdca4ed4ea9151daca52d51e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837823"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="ece7a-103">Operações de serviço de web mensagens unificadas para Exchange</span><span class="sxs-lookup"><span data-stu-id="ece7a-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="ece7a-104">Encontre informações de referência para as operações de serviço web de Unificação de mensagens no Exchange.</span><span class="sxs-lookup"><span data-stu-id="ece7a-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="ece7a-105">O serviço web de Unificação de mensagens oferece muitas operações que permitem que aplicativos de cliente ler e alterar propriedades de Unificação de mensagens, reproduzir mensagens de voz, registre saudações e determinam os itens de caixa de correio sobre dispositivos de telefonia.</span><span class="sxs-lookup"><span data-stu-id="ece7a-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="ece7a-106">Os artigos nesta seção fornecem informações sobre a estrutura geral das mensagens de solicitação e resposta para as operações.</span><span class="sxs-lookup"><span data-stu-id="ece7a-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="ece7a-107">Estes artigos fornecem exemplos que mostram as estruturas de mensagem comuns.</span><span class="sxs-lookup"><span data-stu-id="ece7a-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="ece7a-108">Você pode usar estes exemplos para saber mais sobre o que você pode fazer com uma solicitação de serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ece7a-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ece7a-109">Para versões do Exchange, começando com o Exchange 2010, recomendamos que você use as operações de Unificação de mensagens que estão disponíveis no [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) em vez do serviço web de Unificação de mensagens, pelos seguintes motivos: > baseada no EWS Recursos do Unified Messaging têm suporte de primeira classe na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="ece7a-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons: >  The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="ece7a-110">> Nas versões do Exchange, começando com o Exchange 2010, novos recursos de Unificação de mensagens são adicionados ao EWS, mas não para o serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="ece7a-110">>  In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="ece7a-111">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="ece7a-111">In this section</span></span>
<span data-ttu-id="ece7a-112"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="ece7a-112"></span></span>

- [<span data-ttu-id="ece7a-113">Desconectar a operação (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-113">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-114">Operação de GetCallInfo (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-114">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-115">Operação de GetUMProperties (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-115">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-116">Operação de IsUMEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-116">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-117">Operação de PlayOnPhone (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-117">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-118">Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-118">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-119">Operação de ResetPIN (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-119">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-120">Operação de SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-120">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-121">Operação de SetOofStatus (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-121">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-122">Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-122">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)
    
- [<span data-ttu-id="ece7a-123">Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="ece7a-123">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="ece7a-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="ece7a-124">See also</span></span>

- [<span data-ttu-id="ece7a-125">Referência de serviço de web mensagens unificada para Exchange</span><span class="sxs-lookup"><span data-stu-id="ece7a-125">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="ece7a-126">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="ece7a-126">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="ece7a-127">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="ece7a-127">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

