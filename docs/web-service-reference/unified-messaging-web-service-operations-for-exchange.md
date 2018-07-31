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
ms.openlocfilehash: bd86a4ab2de58e5f04a8d37f17196040bcf38b97
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354355"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="267f0-103">Operações de serviço de web mensagens unificadas para Exchange</span><span class="sxs-lookup"><span data-stu-id="267f0-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="267f0-104">Encontre informações de referência para as operações de serviço web de Unificação de mensagens no Exchange.</span><span class="sxs-lookup"><span data-stu-id="267f0-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="267f0-105">O serviço web de Unificação de mensagens oferece muitas operações que permitem que aplicativos de cliente ler e alterar propriedades de Unificação de mensagens, reproduzir mensagens de voz, registre saudações e determinam os itens de caixa de correio sobre dispositivos de telefonia.</span><span class="sxs-lookup"><span data-stu-id="267f0-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="267f0-106">Os artigos nesta seção fornecem informações sobre a estrutura geral das mensagens de solicitação e resposta para as operações.</span><span class="sxs-lookup"><span data-stu-id="267f0-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="267f0-107">Estes artigos fornecem exemplos que mostram as estruturas de mensagem comuns.</span><span class="sxs-lookup"><span data-stu-id="267f0-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="267f0-108">Você pode usar estes exemplos para saber mais sobre o que você pode fazer com uma solicitação de serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="267f0-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="267f0-109">Para versões do Exchange, começando com o Exchange 2010, recomendamos que você use as operações de Unificação de mensagens que estão disponíveis no [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) em vez do serviço web de Unificação de mensagens, pelos seguintes motivos:</span><span class="sxs-lookup"><span data-stu-id="267f0-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="267f0-110">Os recursos baseados em EWS Unificação de mensagens têm suporte de primeira classe na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="267f0-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="267f0-111">Nas versões do Exchange, começando com o Exchange 2010, novos recursos de Unificação de mensagens são adicionados ao EWS, mas não para o serviço web de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="267f0-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="267f0-112">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="267f0-112">In this section</span></span>
<span data-ttu-id="267f0-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="267f0-113"></span></span>

- [<span data-ttu-id="267f0-114">Operação Disconnect (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="267f0-115">Operação GetCallInfo (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-116">Operação GetUMProperties (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-117">Operação IsUMEnabled (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-118">Operação PlayOnPhone (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-119">Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-120">Operação ResetPIN (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-121">Operação SetMissedCallNotificationEnabled (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="267f0-122">Operação SetOofStatus (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="267f0-123">Operação SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="267f0-124">Operação SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)</span><span class="sxs-lookup"><span data-stu-id="267f0-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="267f0-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="267f0-125">See also</span></span>

- [<span data-ttu-id="267f0-126">Referência de serviço de web mensagens unificada para Exchange</span><span class="sxs-lookup"><span data-stu-id="267f0-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="267f0-127">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="267f0-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="267f0-128">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="267f0-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

