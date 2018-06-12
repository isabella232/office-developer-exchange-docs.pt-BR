---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: O elemento MaxItems Especifica o número máximo de itens para retornar na solicitação.
ms.openlocfilehash: dffb9ba4e29915a65fe2a57b6e7a7b4468028fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824384"
---
# <a name="maxitems"></a><span data-ttu-id="53195-103">MaxItems</span><span class="sxs-lookup"><span data-stu-id="53195-103">MaxItems</span></span>

<span data-ttu-id="53195-104">O elemento **MaxItems** Especifica o número máximo de itens para retornar na solicitação.</span><span class="sxs-lookup"><span data-stu-id="53195-104">The **MaxItems** element specifies the maximum number of items to return in the request.</span></span> 
  
```XML
<MaxItems/>
```

 <span data-ttu-id="53195-105">**int**</span><span class="sxs-lookup"><span data-stu-id="53195-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53195-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="53195-106">Attributes and elements</span></span>

<span data-ttu-id="53195-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53195-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53195-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53195-108">Attributes</span></span>

<span data-ttu-id="53195-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53195-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53195-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53195-110">Child elements</span></span>

<span data-ttu-id="53195-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="53195-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53195-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53195-112">Parent elements</span></span>

[<span data-ttu-id="53195-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="53195-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="53195-114">Text value</span><span class="sxs-lookup"><span data-stu-id="53195-114">Text value</span></span>

<span data-ttu-id="53195-115">O valor de texto do elemento **MaxItems** é o número máximo de itens para retornar na solicitação.</span><span class="sxs-lookup"><span data-stu-id="53195-115">The text value of the **MaxItems** element is the maximum number of items to return in the request.</span></span> <span data-ttu-id="53195-116">Esse número não pode ser menor que zero ou maior que 200.</span><span class="sxs-lookup"><span data-stu-id="53195-116">This number cannot be less than zero or greater than 200.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="53195-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="53195-117">Remarks</span></span>

<span data-ttu-id="53195-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="53195-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="53195-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53195-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53195-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="53195-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53195-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="53195-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="53195-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53195-122">Schema Name</span></span>  <br/> |<span data-ttu-id="53195-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="53195-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="53195-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53195-124">Validation File</span></span>  <br/> |<span data-ttu-id="53195-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="53195-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53195-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="53195-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="53195-127">False</span><span class="sxs-lookup"><span data-stu-id="53195-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53195-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="53195-128">See also</span></span>



[<span data-ttu-id="53195-129">GetReminders</span><span class="sxs-lookup"><span data-stu-id="53195-129">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="53195-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="53195-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

