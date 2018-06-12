---
title: IsNDR
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: O elemento IsNDR indica se as mensagens recebidas devem ser relatórios de falha na entrega (NDRs) em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 651590d055a0532c904dbf6c481dca2f899d673f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824056"
---
# <a name="isndr"></a><span data-ttu-id="20ba3-103">IsNDR</span><span class="sxs-lookup"><span data-stu-id="20ba3-103">IsNDR</span></span>

<span data-ttu-id="20ba3-104">O elemento **IsNDR** indica se as mensagens recebidas devem ser relatórios de falha na entrega (NDRs) em ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="20ba3-104">The **IsNDR** element indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsNDR>true | false</IsNDR>
```

 <span data-ttu-id="20ba3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="20ba3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20ba3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="20ba3-106">Attributes and elements</span></span>

<span data-ttu-id="20ba3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="20ba3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20ba3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="20ba3-108">Attributes</span></span>

<span data-ttu-id="20ba3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="20ba3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20ba3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="20ba3-110">Child elements</span></span>

<span data-ttu-id="20ba3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="20ba3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20ba3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="20ba3-112">Parent elements</span></span>

|<span data-ttu-id="20ba3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20ba3-113">**Element**</span></span>|<span data-ttu-id="20ba3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20ba3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20ba3-115">Condições</span><span class="sxs-lookup"><span data-stu-id="20ba3-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="20ba3-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="20ba3-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="20ba3-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="20ba3-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="20ba3-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="20ba3-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20ba3-119">Text value</span><span class="sxs-lookup"><span data-stu-id="20ba3-119">Text value</span></span>

<span data-ttu-id="20ba3-120">Um valor de texto de **true** indica que a mensagem deve ser uma NDR na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="20ba3-120">A text value of **true** indicates that the message must be an NDR in order for the condition or exception to apply.</span></span> <span data-ttu-id="20ba3-121">Um valor **false** indica que a mensagem não deve ser uma NDR na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="20ba3-121">A value of **false** indicates that the message must not be an NDR in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="20ba3-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="20ba3-122">Remarks</span></span>

<span data-ttu-id="20ba3-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="20ba3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20ba3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="20ba3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20ba3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="20ba3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20ba3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="20ba3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="20ba3-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="20ba3-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20ba3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="20ba3-128">Validation File</span></span>  <br/> |<span data-ttu-id="20ba3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="20ba3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20ba3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="20ba3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="20ba3-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="20ba3-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20ba3-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="20ba3-132">See also</span></span>



- [<span data-ttu-id="20ba3-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="20ba3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
