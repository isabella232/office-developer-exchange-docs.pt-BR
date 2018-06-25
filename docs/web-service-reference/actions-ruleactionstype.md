---
title: Ações (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: O elemento de ações contém uma lista de ações associadas a regras de caixa de entrada.
ms.openlocfilehash: 8ed8095ca8b41e037c2c0dad319c9c4ab99ed2bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751129"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="8acba-103">Ações (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="8acba-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="8acba-104">O elemento de **ações** contém uma lista de ações associadas a regras de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8acba-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="8acba-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="8acba-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8acba-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8acba-106">Attributes and elements</span></span>

<span data-ttu-id="8acba-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8acba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8acba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8acba-108">Attributes</span></span>

<span data-ttu-id="8acba-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8acba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8acba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8acba-110">Child elements</span></span>

<span data-ttu-id="8acba-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Excluir](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead ](markasread.md)  |  [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md)  |  [ StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="8acba-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8acba-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8acba-112">Parent elements</span></span>

[<span data-ttu-id="8acba-113">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8acba-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="8acba-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="8acba-114">Remarks</span></span>

<span data-ttu-id="8acba-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8acba-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8acba-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8acba-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8acba-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8acba-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8acba-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8acba-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8acba-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8acba-119">Schema name</span></span>  <br/> |<span data-ttu-id="8acba-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8acba-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8acba-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8acba-121">Validation file</span></span>  <br/> |<span data-ttu-id="8acba-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8acba-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8acba-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8acba-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8acba-124">false</span><span class="sxs-lookup"><span data-stu-id="8acba-124">false</span></span>  <br/> |
   

