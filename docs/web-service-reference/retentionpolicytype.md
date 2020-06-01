---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: O elemento RetentionPolicyType especifica o tipo de política de retenção aplicado a itens em uma conversa.
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462868"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="9429b-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="9429b-103">RetentionPolicyType</span></span>

<span data-ttu-id="9429b-104">O elemento **RetentionPolicyType** especifica o tipo de política de retenção aplicado a itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="9429b-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="9429b-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="9429b-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9429b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9429b-106">Attributes and elements</span></span>

<span data-ttu-id="9429b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9429b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9429b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9429b-108">Attributes</span></span>

<span data-ttu-id="9429b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9429b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9429b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9429b-110">Child elements</span></span>

<span data-ttu-id="9429b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9429b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9429b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9429b-112">Parent elements</span></span>

[<span data-ttu-id="9429b-113">Conversation</span><span class="sxs-lookup"><span data-stu-id="9429b-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="9429b-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9429b-114">Text value</span></span>

<span data-ttu-id="9429b-115">O valor de texto do elemento **RetentionPolicyType** é o tipo de retenção aplicado a itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="9429b-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="9429b-116">O valor de **delete** indica que os itens na conversa são excluídos quando a retenção expira.</span><span class="sxs-lookup"><span data-stu-id="9429b-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="9429b-117">O valor de texto de **Archive** indica que os itens da conversa serão movidos para a caixa de correio de arquivo morto quando a retenção expirar.</span><span class="sxs-lookup"><span data-stu-id="9429b-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9429b-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="9429b-118">Remarks</span></span>

<span data-ttu-id="9429b-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9429b-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9429b-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9429b-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9429b-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9429b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9429b-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9429b-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9429b-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9429b-123">Schema name</span></span>  <br/> |<span data-ttu-id="9429b-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9429b-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9429b-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9429b-125">Validation file</span></span>  <br/> |<span data-ttu-id="9429b-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9429b-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9429b-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9429b-127">Can be empty</span></span>  <br/> ||
   

