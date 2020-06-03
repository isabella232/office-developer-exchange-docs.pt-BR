---
title: Tipo (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: O elemento Type Especifica o tipo de pasta usado em uma política de retenção.
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465104"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="e548f-103">Tipo (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="e548f-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="e548f-104">O elemento **Type** especifica o tipo de pasta usado em uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="e548f-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="e548f-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="e548f-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e548f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e548f-106">Attributes and elements</span></span>

<span data-ttu-id="e548f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e548f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e548f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e548f-108">Attributes</span></span>

<span data-ttu-id="e548f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e548f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e548f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e548f-110">Child elements</span></span>

<span data-ttu-id="e548f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e548f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e548f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e548f-112">Parent elements</span></span>

[<span data-ttu-id="e548f-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="e548f-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="e548f-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e548f-114">Text value</span></span>

<span data-ttu-id="e548f-115">O valor de texto do elemento **Type** é o tipo de pasta usado em uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="e548f-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="e548f-116">O valor de texto pode ser um dos seguintes valores que representam um tipo de pasta padrão: calendário, contatos, DeletedItems, rascunhos, caixa de entrada, JunkEmail, diário, anotações, caixa de saída, itens enviados, tarefas, todos, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, pessoal, RecoverableItems ou NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="e548f-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e548f-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="e548f-117">Remarks</span></span>

<span data-ttu-id="e548f-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e548f-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e548f-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e548f-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e548f-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e548f-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e548f-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="e548f-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e548f-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e548f-122">Schema name</span></span>  <br/> |<span data-ttu-id="e548f-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e548f-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e548f-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e548f-124">Validation file</span></span>  <br/> |<span data-ttu-id="e548f-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e548f-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e548f-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e548f-126">Can be empty</span></span>  <br/> |<span data-ttu-id="e548f-127">falso</span><span class="sxs-lookup"><span data-stu-id="e548f-127">false</span></span>  <br/> |
   

