---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: O elemento IsInError indica se a regra está em uma condição de erro.
ms.openlocfilehash: 9f77bbe11106174d0e82c5257e08c3728d67c60c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824033"
---
# <a name="isinerror"></a><span data-ttu-id="52143-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="52143-103">IsInError</span></span>

<span data-ttu-id="52143-104">O elemento **IsInError** indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="52143-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="52143-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="52143-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52143-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="52143-106">Attributes and elements</span></span>

<span data-ttu-id="52143-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="52143-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52143-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="52143-108">Attributes</span></span>

<span data-ttu-id="52143-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="52143-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52143-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="52143-110">Child elements</span></span>

<span data-ttu-id="52143-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="52143-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="52143-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="52143-112">Parent elements</span></span>

|<span data-ttu-id="52143-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="52143-113">**Element**</span></span>|<span data-ttu-id="52143-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52143-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52143-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="52143-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="52143-116">Representa uma regra de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="52143-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="52143-117">Text value</span><span class="sxs-lookup"><span data-stu-id="52143-117">Text value</span></span>

<span data-ttu-id="52143-118">Um valor de texto de **true** indica que a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="52143-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="52143-119">Um valor **false** indica que a regra não está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="52143-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="52143-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="52143-120">Remarks</span></span>

<span data-ttu-id="52143-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="52143-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52143-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="52143-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52143-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="52143-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="52143-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="52143-124">Schema Name</span></span>  <br/> |<span data-ttu-id="52143-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="52143-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="52143-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="52143-126">Validation File</span></span>  <br/> |<span data-ttu-id="52143-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="52143-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="52143-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="52143-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="52143-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="52143-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52143-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="52143-130">See also</span></span>



- [<span data-ttu-id="52143-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52143-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

