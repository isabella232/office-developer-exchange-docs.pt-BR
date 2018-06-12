---
title: RuleId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleId
api_type:
- schema
ms.assetid: 456e3c34-e536-456a-ac40-7fd4f94c0bad
description: O elemento RuleId Especifica um identificador de regra.
ms.openlocfilehash: 4dfa71c9fb6ee362d776487952199f2430e5e4a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825260"
---
# <a name="ruleid"></a><span data-ttu-id="cf368-103">RuleId</span><span class="sxs-lookup"><span data-stu-id="cf368-103">RuleId</span></span>

<span data-ttu-id="cf368-104">O elemento **RuleId** Especifica um identificador de regra.</span><span class="sxs-lookup"><span data-stu-id="cf368-104">The **RuleId** element specifies a rule identifier.</span></span> 
  
```XML
<RuleId/>
```

 <span data-ttu-id="cf368-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="cf368-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf368-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cf368-106">Attributes and elements</span></span>

<span data-ttu-id="cf368-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf368-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf368-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf368-108">Attributes</span></span>

<span data-ttu-id="cf368-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf368-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf368-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf368-110">Child elements</span></span>

<span data-ttu-id="cf368-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf368-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf368-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf368-112">Parent elements</span></span>

|<span data-ttu-id="cf368-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf368-113">**Element**</span></span>|<span data-ttu-id="cf368-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf368-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf368-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="cf368-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="cf368-116">Representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf368-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cf368-117">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="cf368-117">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="cf368-118">Representa a operação para excluir uma regra de caixa de entrada existente.</span><span class="sxs-lookup"><span data-stu-id="cf368-118">Represents the operation to delete an existing Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf368-119">Text value</span><span class="sxs-lookup"><span data-stu-id="cf368-119">Text value</span></span>

<span data-ttu-id="cf368-120">O valor de texto é um valor string que representa a regra.</span><span class="sxs-lookup"><span data-stu-id="cf368-120">The text value is a string value that represents the rule.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf368-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf368-121">Remarks</span></span>

<span data-ttu-id="cf368-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf368-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf368-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cf368-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf368-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf368-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cf368-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf368-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cf368-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cf368-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cf368-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf368-127">Validation File</span></span>  <br/> |<span data-ttu-id="cf368-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf368-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf368-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf368-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf368-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="cf368-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf368-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="cf368-131">See also</span></span>



- [<span data-ttu-id="cf368-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cf368-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

