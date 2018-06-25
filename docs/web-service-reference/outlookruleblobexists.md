---
title: OutlookRuleBlobExists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: O elemento OutlookRuleBlobExists indica se um blob de regra do Microsoft Outlook existe na caixa de correio do usuário.
ms.openlocfilehash: a738377cd3c1d69b90ac39ca479b03b3220d5bc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824679"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="77e10-103">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="77e10-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="77e10-104">O elemento **OutlookRuleBlobExists** indica se um blob de regra do Microsoft Outlook existe na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="77e10-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="77e10-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="77e10-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="77e10-106">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="77e10-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="77e10-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="77e10-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77e10-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="77e10-108">Attributes and elements</span></span>

<span data-ttu-id="77e10-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77e10-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77e10-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="77e10-110">Attributes</span></span>

<span data-ttu-id="77e10-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77e10-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77e10-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77e10-112">Child elements</span></span>

<span data-ttu-id="77e10-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77e10-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="77e10-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77e10-114">Parent elements</span></span>

|<span data-ttu-id="77e10-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77e10-115">**Element**</span></span>|<span data-ttu-id="77e10-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77e10-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77e10-117">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="77e10-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="77e10-118">Representa uma resposta a uma solicitação de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="77e10-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77e10-119">Text value</span><span class="sxs-lookup"><span data-stu-id="77e10-119">Text value</span></span>

<span data-ttu-id="77e10-120">Um valor de texto de **true** indica a existência de um blob de regra do Outlook.</span><span class="sxs-lookup"><span data-stu-id="77e10-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="77e10-121">Um valor de texto de **false** indica que não existe um blob de regra do Outlook.</span><span class="sxs-lookup"><span data-stu-id="77e10-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="77e10-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="77e10-122">Remarks</span></span>

<span data-ttu-id="77e10-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77e10-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77e10-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="77e10-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77e10-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="77e10-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="77e10-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77e10-126">Schema Name</span></span>  <br/> |<span data-ttu-id="77e10-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="77e10-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="77e10-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77e10-128">Validation File</span></span>  <br/> |<span data-ttu-id="77e10-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="77e10-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="77e10-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77e10-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="77e10-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="77e10-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77e10-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="77e10-132">See also</span></span>



- [<span data-ttu-id="77e10-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77e10-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

