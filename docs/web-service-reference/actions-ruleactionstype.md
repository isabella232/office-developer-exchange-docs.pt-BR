---
title: Ações (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: O elemento Actions contém uma lista de ações associadas às regras de caixa de entrada.
ms.openlocfilehash: fbef3b69b1688d7c612af018d6a19f9ec1728066
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529676"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="0bd27-103">Ações (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="0bd27-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="0bd27-104">O elemento **Actions** contém uma lista de ações associadas às regras de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="0bd27-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
```XML
<Actions>
   <AssignCategories/>
   <CopyToFolder/>
   <Delete/>
   <ForwardAsAttachmentToRecipients/>
   <ForwardToRecipients/>
   <MarkImportance/>
   <MarkAsRead/>
   <MoveToFolder/>
   <PermanentDelete/>
   <RedirectToRecipients/>
   <SendSMSAlertToRecipients/>
   <ServerReplyWithMessage/>
   <StopProcessingRules/>
</Actions>
```

 <span data-ttu-id="0bd27-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="0bd27-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bd27-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0bd27-106">Attributes and elements</span></span>

<span data-ttu-id="0bd27-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0bd27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bd27-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0bd27-108">Attributes</span></span>

<span data-ttu-id="0bd27-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0bd27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bd27-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0bd27-110">Child elements</span></span>

<span data-ttu-id="0bd27-111">[AssignCategories](assigncategories.md)  |  [CopyToFolder](copytofolder.md)  |  [Excluir](delete.md)  |  [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md)  |  [ForwardToRecipients](forwardtorecipients.md)  |  [MarkImportance](markimportance.md)  |  [MarkAsRead](markasread.md)  |  [MoveToFolder](movetofolder.md)  |  [PermanentDelete](permanentdelete.md)  |  [RedirectToRecipients](redirecttorecipients.md)  |  [SendSMSAlertToRecipients](sendsmsalerttorecipients.md)  |  [ServerReplyWithMessage](serverreplywithmessage.md)  |  [StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="0bd27-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bd27-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0bd27-112">Parent elements</span></span>

[<span data-ttu-id="0bd27-113">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="0bd27-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="0bd27-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="0bd27-114">Remarks</span></span>

<span data-ttu-id="0bd27-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0bd27-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0bd27-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bd27-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bd27-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0bd27-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bd27-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bd27-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bd27-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0bd27-119">Schema name</span></span>  <br/> |<span data-ttu-id="0bd27-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0bd27-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bd27-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0bd27-121">Validation file</span></span>  <br/> |<span data-ttu-id="0bd27-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0bd27-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bd27-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0bd27-123">Can be empty</span></span>  <br/> |<span data-ttu-id="0bd27-124">falso</span><span class="sxs-lookup"><span data-stu-id="0bd27-124">false</span></span>  <br/> |
   

