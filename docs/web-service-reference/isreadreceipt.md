---
title: IsReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: O elemento IsReadReceipt indica se as mensagens de entrada devem ser confirmações de leitura para que a condição ou exceção seja aplicada.
ms.openlocfilehash: e86a7776bc43204dae9fc92f21d4304255ddb888
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463899"
---
# <a name="isreadreceipt"></a><span data-ttu-id="29bc0-103">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="29bc0-103">IsReadReceipt</span></span>

<span data-ttu-id="29bc0-104">O elemento **IsReadReceipt** indica se as mensagens de entrada devem ser confirmações de leitura para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="29bc0-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="29bc0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="29bc0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29bc0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="29bc0-106">Attributes and elements</span></span>

<span data-ttu-id="29bc0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="29bc0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29bc0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="29bc0-108">Attributes</span></span>

<span data-ttu-id="29bc0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29bc0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29bc0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="29bc0-110">Child elements</span></span>

<span data-ttu-id="29bc0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="29bc0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29bc0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="29bc0-112">Parent elements</span></span>

|<span data-ttu-id="29bc0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="29bc0-113">**Element**</span></span>|<span data-ttu-id="29bc0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="29bc0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29bc0-115">Condições</span><span class="sxs-lookup"><span data-stu-id="29bc0-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="29bc0-116">Representa as condições que, ao serem atendidas, dispararão as ações de regra para essa regra.</span><span class="sxs-lookup"><span data-stu-id="29bc0-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="29bc0-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="29bc0-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="29bc0-118">Representa todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="29bc0-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29bc0-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="29bc0-119">Text value</span></span>

<span data-ttu-id="29bc0-120">Um valor de texto **true** indica que a mensagem deve ser uma confirmação de leitura para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="29bc0-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="29bc0-121">Se a mensagem não tiver que ser uma confirmação de leitura para a condição ou exceção a ser aplicada, o valor será **false**.</span><span class="sxs-lookup"><span data-stu-id="29bc0-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29bc0-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="29bc0-122">Remarks</span></span>

<span data-ttu-id="29bc0-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="29bc0-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29bc0-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="29bc0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29bc0-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="29bc0-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29bc0-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="29bc0-126">Schema Name</span></span>  <br/> |<span data-ttu-id="29bc0-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="29bc0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="29bc0-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="29bc0-128">Validation File</span></span>  <br/> |<span data-ttu-id="29bc0-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29bc0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29bc0-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="29bc0-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="29bc0-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="29bc0-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29bc0-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="29bc0-132">See also</span></span>



- [<span data-ttu-id="29bc0-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="29bc0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

