---
title: Tipo (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: O elemento Type especifica o tipo da pasta usada em uma política de retenção.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837804"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="e4ef0-103">Tipo (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="e4ef0-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="e4ef0-104">O **tipo** de elemento Especifica o tipo da pasta usada em uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="e4ef0-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="e4ef0-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4ef0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e4ef0-106">Attributes and elements</span></span>

<span data-ttu-id="e4ef0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4ef0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e4ef0-108">Attributes</span></span>

<span data-ttu-id="e4ef0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4ef0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e4ef0-110">Child elements</span></span>

<span data-ttu-id="e4ef0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4ef0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e4ef0-112">Parent elements</span></span>

[<span data-ttu-id="e4ef0-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="e4ef0-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="e4ef0-114">Text value</span><span class="sxs-lookup"><span data-stu-id="e4ef0-114">Text value</span></span>

<span data-ttu-id="e4ef0-115">O valor de texto do elemento **Type** é o tipo de pasta usado em uma política de retenção.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="e4ef0-116">O valor de texto pode ser um dos seguintes valores que representam um tipo de pasta padrão: calendário, contatos, DeletedItems, Rascunhos, caixa de entrada, JunkEmail, diário, anotações, caixa de saída, itens enviados, tarefas, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, pessoal, RecoverableItems ou NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="e4ef0-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e4ef0-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e4ef0-117">Remarks</span></span>

<span data-ttu-id="e4ef0-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e4ef0-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4ef0-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4ef0-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e4ef0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4ef0-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4ef0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4ef0-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e4ef0-122">Schema name</span></span>  <br/> |<span data-ttu-id="e4ef0-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e4ef0-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4ef0-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e4ef0-124">Validation file</span></span>  <br/> |<span data-ttu-id="e4ef0-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4ef0-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4ef0-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e4ef0-126">Can be empty</span></span>  <br/> |<span data-ttu-id="e4ef0-127">false</span><span class="sxs-lookup"><span data-stu-id="e4ef0-127">false</span></span>  <br/> |
   

