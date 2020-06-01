---
title: FromConnectedAccounts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: O elemento FromConnectedAccounts representa os nomes de conta de email dos quais as mensagens de entrada precisam ter sido agregadas para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 159ae064827c2f9c2b470580ad5457264e8dae93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464046"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="c10a6-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="c10a6-103">FromConnectedAccounts</span></span>

<span data-ttu-id="c10a6-104">O elemento **FromConnectedAccounts** representa os nomes de conta de email dos quais as mensagens de entrada precisam ter sido agregadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="c10a6-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="c10a6-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c10a6-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c10a6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c10a6-106">Attributes and elements</span></span>

<span data-ttu-id="c10a6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c10a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c10a6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c10a6-108">Attributes</span></span>

<span data-ttu-id="c10a6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c10a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c10a6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c10a6-110">Child elements</span></span>

|<span data-ttu-id="c10a6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c10a6-111">**Element**</span></span>|<span data-ttu-id="c10a6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c10a6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c10a6-113">String</span><span class="sxs-lookup"><span data-stu-id="c10a6-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c10a6-114">Representa um nome de conta de email a partir do qual as mensagens de entrada precisam ser agregadas para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="c10a6-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c10a6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c10a6-115">Parent elements</span></span>

|<span data-ttu-id="c10a6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c10a6-116">**Element**</span></span>|<span data-ttu-id="c10a6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c10a6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c10a6-118">Condições</span><span class="sxs-lookup"><span data-stu-id="c10a6-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c10a6-119">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="c10a6-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c10a6-120">Exceções</span><span class="sxs-lookup"><span data-stu-id="c10a6-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c10a6-121">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="c10a6-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c10a6-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c10a6-122">Text value</span></span>

<span data-ttu-id="c10a6-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c10a6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c10a6-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c10a6-124">Remarks</span></span>

<span data-ttu-id="c10a6-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c10a6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c10a6-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c10a6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c10a6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c10a6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c10a6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c10a6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c10a6-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c10a6-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c10a6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c10a6-130">Validation File</span></span>  <br/> |<span data-ttu-id="c10a6-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c10a6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c10a6-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c10a6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c10a6-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c10a6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c10a6-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="c10a6-134">See also</span></span>



- [<span data-ttu-id="c10a6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c10a6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

