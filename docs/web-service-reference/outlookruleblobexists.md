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
description: O elemento OutlookRuleBlobExists indica se existe um blob de regra do Microsoft Outlook na caixa de correio do usuário.
ms.openlocfilehash: 6a5c2a2ec0246d38b22279b86772972ea81922c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529025"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="93aa2-103">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="93aa2-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="93aa2-104">O elemento **OutlookRuleBlobExists** indica se existe um blob de regra do Microsoft Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="93aa2-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="93aa2-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="93aa2-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="93aa2-106">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="93aa2-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="93aa2-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="93aa2-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93aa2-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="93aa2-108">Attributes and elements</span></span>

<span data-ttu-id="93aa2-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="93aa2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93aa2-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="93aa2-110">Attributes</span></span>

<span data-ttu-id="93aa2-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93aa2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93aa2-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="93aa2-112">Child elements</span></span>

<span data-ttu-id="93aa2-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93aa2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93aa2-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="93aa2-114">Parent elements</span></span>

|<span data-ttu-id="93aa2-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93aa2-115">**Element**</span></span>|<span data-ttu-id="93aa2-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93aa2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93aa2-117">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="93aa2-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="93aa2-118">Representa uma resposta a uma solicitação de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="93aa2-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93aa2-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="93aa2-119">Text value</span></span>

<span data-ttu-id="93aa2-120">Um valor de texto **true** indica que um blob de regra do Outlook existe.</span><span class="sxs-lookup"><span data-stu-id="93aa2-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="93aa2-121">Um valor de texto **false** indica que um blob de regra do Outlook não existe.</span><span class="sxs-lookup"><span data-stu-id="93aa2-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="93aa2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="93aa2-122">Remarks</span></span>

<span data-ttu-id="93aa2-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="93aa2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93aa2-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="93aa2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93aa2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="93aa2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93aa2-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="93aa2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="93aa2-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="93aa2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93aa2-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="93aa2-128">Validation File</span></span>  <br/> |<span data-ttu-id="93aa2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93aa2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93aa2-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="93aa2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="93aa2-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="93aa2-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93aa2-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="93aa2-132">See also</span></span>



- [<span data-ttu-id="93aa2-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="93aa2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

