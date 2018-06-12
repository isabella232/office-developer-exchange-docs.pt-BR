---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: O elemento RetentionPolicyType Especifica o tipo de política de retenção aplicado aos itens em uma conversa.
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825229"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="2e2b9-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2e2b9-103">RetentionPolicyType</span></span>

<span data-ttu-id="2e2b9-104">O elemento **RetentionPolicyType** Especifica o tipo de política de retenção aplicado aos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="2e2b9-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="2e2b9-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e2b9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2e2b9-106">Attributes and elements</span></span>

<span data-ttu-id="2e2b9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e2b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e2b9-108">Attributes</span></span>

<span data-ttu-id="2e2b9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e2b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e2b9-110">Child elements</span></span>

<span data-ttu-id="2e2b9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e2b9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e2b9-112">Parent elements</span></span>

[<span data-ttu-id="2e2b9-113">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="2e2b9-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="2e2b9-114">Text value</span><span class="sxs-lookup"><span data-stu-id="2e2b9-114">Text value</span></span>

<span data-ttu-id="2e2b9-115">O valor de texto do elemento **RetentionPolicyType** é o tipo de retenção aplicado aos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="2e2b9-116">O valor de **Excluir** texto indica que os itens da conversa são excluídos quando o status em retenção expira.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="2e2b9-117">O valor de texto do **Archive** indica que os itens da conversa serão movidos para a caixa de correio de arquivo morto quando o status em retenção expira.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2e2b9-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2e2b9-118">Remarks</span></span>

<span data-ttu-id="2e2b9-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e2b9-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e2b9-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e2b9-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2e2b9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e2b9-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e2b9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e2b9-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e2b9-123">Schema name</span></span>  <br/> |<span data-ttu-id="2e2b9-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2e2b9-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e2b9-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e2b9-125">Validation file</span></span>  <br/> |<span data-ttu-id="2e2b9-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2e2b9-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e2b9-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2e2b9-127">Can be empty</span></span>  <br/> ||
   

