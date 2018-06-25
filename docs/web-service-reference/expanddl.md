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
description: O elemento de ExpandDL define uma solicitação para expandir uma lista de distribuição.
ms.openlocfilehash: ef93ed4684427a74a4fd2c38b4020ecb743fbaaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752137"
---
# <a name="expanddl"></a><span data-ttu-id="3fc15-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="3fc15-103">ExpandDL</span></span>

<span data-ttu-id="3fc15-104">O elemento de **ExpandDL** define uma solicitação para expandir uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="3fc15-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="3fc15-105">**ExpandDLType**</span><span class="sxs-lookup"><span data-stu-id="3fc15-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fc15-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3fc15-106">Attributes and elements</span></span>

<span data-ttu-id="3fc15-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3fc15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fc15-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3fc15-108">Attributes</span></span>

<span data-ttu-id="3fc15-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3fc15-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fc15-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3fc15-110">Child elements</span></span>

|<span data-ttu-id="3fc15-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3fc15-111">**Element**</span></span>|<span data-ttu-id="3fc15-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3fc15-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fc15-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="3fc15-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3fc15-114">Identifica um endereço de email totalmente resolvido ou uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="3fc15-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="3fc15-115">Esta caixa de correio representa para expandir a lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="3fc15-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fc15-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3fc15-116">Parent elements</span></span>

<span data-ttu-id="3fc15-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fc15-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3fc15-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="3fc15-118">Remarks</span></span>

<span data-ttu-id="3fc15-119">A expansão de lista de distribuição será executada apenas para uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="3fc15-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="3fc15-120">A expansão de lista de distribuição não é recursiva.</span><span class="sxs-lookup"><span data-stu-id="3fc15-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="3fc15-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3fc15-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fc15-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3fc15-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fc15-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3fc15-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3fc15-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3fc15-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3fc15-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="3fc15-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="3fc15-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3fc15-126">Validation File</span></span>  <br/> |<span data-ttu-id="3fc15-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3fc15-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3fc15-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3fc15-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fc15-129">False</span><span class="sxs-lookup"><span data-stu-id="3fc15-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fc15-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="3fc15-130">See also</span></span>



[<span data-ttu-id="3fc15-131">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="3fc15-131">ExpandDL operation</span></span>](expanddl-operation.md)

