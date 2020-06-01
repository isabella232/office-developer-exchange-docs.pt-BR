---
title: Prioridade
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: O elemento Priority indica a ordem na qual uma regra deve ser executada.
ms.openlocfilehash: a5a894bba583618dd04430fc89f125c8920b0202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462399"
---
# <a name="priority"></a><span data-ttu-id="03bc2-103">Prioridade</span><span class="sxs-lookup"><span data-stu-id="03bc2-103">Priority</span></span>

<span data-ttu-id="03bc2-104">O elemento **Priority** indica a ordem na qual uma regra deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="03bc2-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="03bc2-105">**int**</span><span class="sxs-lookup"><span data-stu-id="03bc2-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03bc2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="03bc2-106">Attributes and elements</span></span>

<span data-ttu-id="03bc2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="03bc2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03bc2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="03bc2-108">Attributes</span></span>

<span data-ttu-id="03bc2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03bc2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03bc2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="03bc2-110">Child elements</span></span>

<span data-ttu-id="03bc2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="03bc2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03bc2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="03bc2-112">Parent elements</span></span>

|<span data-ttu-id="03bc2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03bc2-113">**Element**</span></span>|<span data-ttu-id="03bc2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03bc2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03bc2-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="03bc2-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="03bc2-116">Representa uma regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="03bc2-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03bc2-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="03bc2-117">Text value</span></span>

<span data-ttu-id="03bc2-118">O valor de texto para o elemento **Priority** é um inteiro que indica a ordem de execução na qual uma regra deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="03bc2-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="03bc2-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="03bc2-119">Remarks</span></span>

<span data-ttu-id="03bc2-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="03bc2-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03bc2-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="03bc2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03bc2-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="03bc2-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03bc2-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="03bc2-123">Schema Name</span></span>  <br/> |<span data-ttu-id="03bc2-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="03bc2-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03bc2-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="03bc2-125">Validation File</span></span>  <br/> |<span data-ttu-id="03bc2-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="03bc2-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03bc2-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="03bc2-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="03bc2-128">False</span><span class="sxs-lookup"><span data-stu-id="03bc2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03bc2-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="03bc2-129">See also</span></span>



- [<span data-ttu-id="03bc2-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03bc2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

