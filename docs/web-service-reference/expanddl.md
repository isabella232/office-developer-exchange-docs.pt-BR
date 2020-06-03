---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: O elemento ExpandDL define uma solicitação para expandir uma lista de distribuição.
ms.openlocfilehash: 52b1ea1b51ce185c7a266e3002a4484e4b813bc0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456931"
---
# <a name="expanddl"></a><span data-ttu-id="e74c7-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="e74c7-103">ExpandDL</span></span>

<span data-ttu-id="e74c7-104">O elemento **ExpandDL** define uma solicitação para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e74c7-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="e74c7-105">**ExpandDLType**</span><span class="sxs-lookup"><span data-stu-id="e74c7-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e74c7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e74c7-106">Attributes and elements</span></span>

<span data-ttu-id="e74c7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e74c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e74c7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e74c7-108">Attributes</span></span>

<span data-ttu-id="e74c7-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e74c7-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e74c7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e74c7-110">Child elements</span></span>

|<span data-ttu-id="e74c7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e74c7-111">**Element**</span></span>|<span data-ttu-id="e74c7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e74c7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e74c7-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="e74c7-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e74c7-114">Identifica um endereço de email totalmente resolvido ou uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e74c7-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="e74c7-115">Esta caixa de correio representa a lista de distribuição a ser expandida.</span><span class="sxs-lookup"><span data-stu-id="e74c7-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e74c7-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e74c7-116">Parent elements</span></span>

<span data-ttu-id="e74c7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e74c7-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e74c7-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="e74c7-118">Remarks</span></span>

<span data-ttu-id="e74c7-119">Uma expansão de lista de distribuição só será executada para uma única lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e74c7-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="e74c7-120">Uma expansão de lista de distribuição não é recursiva.</span><span class="sxs-lookup"><span data-stu-id="e74c7-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="e74c7-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e74c7-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e74c7-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e74c7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e74c7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e74c7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e74c7-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e74c7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e74c7-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e74c7-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="e74c7-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e74c7-126">Validation File</span></span>  <br/> |<span data-ttu-id="e74c7-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e74c7-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e74c7-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e74c7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e74c7-129">False</span><span class="sxs-lookup"><span data-stu-id="e74c7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e74c7-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="e74c7-130">See also</span></span>



[<span data-ttu-id="e74c7-131">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="e74c7-131">ExpandDL operation</span></span>](expanddl-operation.md)

