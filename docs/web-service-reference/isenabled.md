---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: O elemento IsEnabled indica se a regra está habilitada.
ms.openlocfilehash: 7a150dc4a27cf4ff7da9825d1daae2b747088539
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455307"
---
# <a name="isenabled"></a><span data-ttu-id="0408e-103">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="0408e-103">IsEnabled</span></span>

<span data-ttu-id="0408e-104">O elemento **IsEnabled** indica se a regra está habilitada.</span><span class="sxs-lookup"><span data-stu-id="0408e-104">The **IsEnabled** element indicates whether the rule is enabled.</span></span> 
  
```XML
<IsEnabled/>
```

 <span data-ttu-id="0408e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0408e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0408e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0408e-106">Attributes and elements</span></span>

<span data-ttu-id="0408e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0408e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0408e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0408e-108">Attributes</span></span>

<span data-ttu-id="0408e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0408e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0408e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0408e-110">Child elements</span></span>

<span data-ttu-id="0408e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0408e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0408e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0408e-112">Parent elements</span></span>

|<span data-ttu-id="0408e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0408e-113">**Element**</span></span>|<span data-ttu-id="0408e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0408e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0408e-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="0408e-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="0408e-116">Representa uma regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0408e-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0408e-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0408e-117">Text value</span></span>

<span data-ttu-id="0408e-118">Um valor de texto **true** indica que a regra está habilitada e pode ser executada.</span><span class="sxs-lookup"><span data-stu-id="0408e-118">A text value of **true** indicates that the rule is enabled and can be executed.</span></span> <span data-ttu-id="0408e-119">Um valor **false** indica que a regra não pode ser executada.</span><span class="sxs-lookup"><span data-stu-id="0408e-119">A value of **false** indicates that the rule cannot be executed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0408e-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="0408e-120">Remarks</span></span>

<span data-ttu-id="0408e-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0408e-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0408e-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0408e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0408e-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="0408e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0408e-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0408e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0408e-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0408e-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0408e-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0408e-126">Validation File</span></span>  <br/> |<span data-ttu-id="0408e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0408e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0408e-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0408e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0408e-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0408e-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0408e-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0408e-130">See also</span></span>



- [<span data-ttu-id="0408e-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0408e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

