---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: O elemento IsNotSupported indica se a regra não pode ser modificada usando as APIs de código gerenciado.
ms.openlocfilehash: e2d0c506209978fd5e8702e0de6cddf2e9c4b7fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465832"
---
# <a name="isnotsupported"></a><span data-ttu-id="4cc71-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="4cc71-103">IsNotSupported</span></span>

<span data-ttu-id="4cc71-104">O elemento **IsNotSupported** indica se a regra não pode ser modificada usando as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4cc71-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="4cc71-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4cc71-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cc71-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4cc71-106">Attributes and elements</span></span>

<span data-ttu-id="4cc71-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4cc71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cc71-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4cc71-108">Attributes</span></span>

<span data-ttu-id="4cc71-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cc71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cc71-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4cc71-110">Child elements</span></span>

<span data-ttu-id="4cc71-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4cc71-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4cc71-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4cc71-112">Parent elements</span></span>

|<span data-ttu-id="4cc71-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4cc71-113">**Element**</span></span>|<span data-ttu-id="4cc71-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4cc71-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cc71-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="4cc71-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="4cc71-116">Representa uma regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4cc71-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4cc71-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4cc71-117">Text value</span></span>

<span data-ttu-id="4cc71-118">Um valor **true** indica que a regra não pode ser modificada usando as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4cc71-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="4cc71-119">Um valor **false** indica que a regra pode ser modificada usando as APIs de código gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4cc71-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4cc71-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4cc71-120">Remarks</span></span>

<span data-ttu-id="4cc71-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cc71-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cc71-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4cc71-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cc71-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="4cc71-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4cc71-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4cc71-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4cc71-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4cc71-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4cc71-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4cc71-126">Validation File</span></span>  <br/> |<span data-ttu-id="4cc71-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4cc71-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cc71-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4cc71-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cc71-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4cc71-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cc71-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4cc71-130">See also</span></span>



- [<span data-ttu-id="4cc71-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4cc71-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

