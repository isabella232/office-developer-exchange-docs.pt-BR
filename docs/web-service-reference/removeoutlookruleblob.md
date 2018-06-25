---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: O elemento RemoveOutlookRuleBlob indica se deseja remover o blob de regra do Microsoft Outlook.
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825102"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="55739-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="55739-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="55739-104">O elemento **RemoveOutlookRuleBlob** indica se deseja remover o blob de regra do Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="55739-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="55739-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="55739-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="55739-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="55739-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="55739-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="55739-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55739-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="55739-108">Attributes and elements</span></span>

<span data-ttu-id="55739-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="55739-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55739-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="55739-110">Attributes</span></span>

<span data-ttu-id="55739-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="55739-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55739-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="55739-112">Child elements</span></span>

<span data-ttu-id="55739-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="55739-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55739-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="55739-114">Parent elements</span></span>

|<span data-ttu-id="55739-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55739-115">**Element**</span></span>|<span data-ttu-id="55739-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55739-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55739-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="55739-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="55739-118">Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no armazenamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="55739-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55739-119">Text value</span><span class="sxs-lookup"><span data-stu-id="55739-119">Text value</span></span>

<span data-ttu-id="55739-120">Um valor de texto de **true** indica que o blob de regra do Outlook deve ser removido.</span><span class="sxs-lookup"><span data-stu-id="55739-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="55739-121">Um valor de texto de **false** indica que o blob de regra do Outlook não deve ser removido.</span><span class="sxs-lookup"><span data-stu-id="55739-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55739-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="55739-122">Remarks</span></span>

<span data-ttu-id="55739-123">Defina esse elemento como **true** para permitir uma atualização de regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="55739-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="55739-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="55739-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55739-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="55739-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55739-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="55739-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55739-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="55739-127">Schema Name</span></span>  <br/> |<span data-ttu-id="55739-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="55739-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="55739-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="55739-129">Validation File</span></span>  <br/> |<span data-ttu-id="55739-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55739-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55739-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="55739-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="55739-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="55739-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55739-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="55739-133">See also</span></span>



[<span data-ttu-id="55739-134">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="55739-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="55739-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="55739-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

