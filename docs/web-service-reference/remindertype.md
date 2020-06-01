---
title: Remindertype
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: O elemento remindertype especifica o tipo de lembretes a ser retornado.
ms.openlocfilehash: 4ac20143bbfb29fb8f962515f2faba224b2f973f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465524"
---
# <a name="remindertype"></a><span data-ttu-id="31bd3-103">Remindertype</span><span class="sxs-lookup"><span data-stu-id="31bd3-103">ReminderType</span></span>

<span data-ttu-id="31bd3-104">O elemento **Remindertype** especifica o tipo de lembretes a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="31bd3-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="31bd3-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="31bd3-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31bd3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="31bd3-106">Attributes and elements</span></span>

<span data-ttu-id="31bd3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31bd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31bd3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="31bd3-108">Attributes</span></span>

<span data-ttu-id="31bd3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31bd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31bd3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31bd3-110">Child elements</span></span>

<span data-ttu-id="31bd3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31bd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31bd3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31bd3-112">Parent elements</span></span>

[<span data-ttu-id="31bd3-113">Getlembretes</span><span class="sxs-lookup"><span data-stu-id="31bd3-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="31bd3-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="31bd3-114">Text value</span></span>

<span data-ttu-id="31bd3-115">O valor de texto do elemento **Remindertype** é o tipo de lembretes a ser retornado, **tudo**, **atual**ou **antigo**.</span><span class="sxs-lookup"><span data-stu-id="31bd3-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="31bd3-116">**All** é o valor recomendado para este elemento.</span><span class="sxs-lookup"><span data-stu-id="31bd3-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="31bd3-117">Para obter mais informações sobre a relação entre o elemento **Remindertype** e os elementos [BeginTime](begintime.md) e [EndTime](endtime-remindermessagedatatype.md) , consulte [getlembrations Operation](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="31bd3-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31bd3-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="31bd3-118">Remarks</span></span>

<span data-ttu-id="31bd3-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31bd3-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31bd3-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31bd3-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31bd3-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="31bd3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31bd3-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="31bd3-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="31bd3-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="31bd3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="31bd3-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="31bd3-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="31bd3-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="31bd3-125">Validation File</span></span>  <br/> |<span data-ttu-id="31bd3-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="31bd3-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="31bd3-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="31bd3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="31bd3-128">False</span><span class="sxs-lookup"><span data-stu-id="31bd3-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31bd3-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="31bd3-129">See also</span></span>



[<span data-ttu-id="31bd3-130">Getlembretes</span><span class="sxs-lookup"><span data-stu-id="31bd3-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="31bd3-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="31bd3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

