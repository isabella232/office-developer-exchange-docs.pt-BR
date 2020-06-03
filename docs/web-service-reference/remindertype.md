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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465524"
---
# <a name="remindertype"></a><span data-ttu-id="faa5a-103">Remindertype</span><span class="sxs-lookup"><span data-stu-id="faa5a-103">ReminderType</span></span>

<span data-ttu-id="faa5a-104">O elemento **Remindertype** especifica o tipo de lembretes a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="faa5a-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="faa5a-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="faa5a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faa5a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="faa5a-106">Attributes and elements</span></span>

<span data-ttu-id="faa5a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="faa5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faa5a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="faa5a-108">Attributes</span></span>

<span data-ttu-id="faa5a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="faa5a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="faa5a-110">Child elements</span></span>

<span data-ttu-id="faa5a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="faa5a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="faa5a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="faa5a-112">Parent elements</span></span>

[<span data-ttu-id="faa5a-113">Getlembretes</span><span class="sxs-lookup"><span data-stu-id="faa5a-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="faa5a-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="faa5a-114">Text value</span></span>

<span data-ttu-id="faa5a-115">O valor de texto do elemento **Remindertype** é o tipo de lembretes a ser retornado, **tudo**, **atual**ou **antigo**.</span><span class="sxs-lookup"><span data-stu-id="faa5a-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="faa5a-116">**All** é o valor recomendado para este elemento.</span><span class="sxs-lookup"><span data-stu-id="faa5a-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="faa5a-117">Para obter mais informações sobre a relação entre o elemento **Remindertype** e os elementos [BeginTime](begintime.md) e [EndTime](endtime-remindermessagedatatype.md) , consulte [getlembrations Operation](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="faa5a-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="faa5a-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="faa5a-118">Remarks</span></span>

<span data-ttu-id="faa5a-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="faa5a-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="faa5a-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="faa5a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faa5a-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="faa5a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faa5a-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="faa5a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="faa5a-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="faa5a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="faa5a-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="faa5a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="faa5a-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="faa5a-125">Validation File</span></span>  <br/> |<span data-ttu-id="faa5a-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="faa5a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="faa5a-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="faa5a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="faa5a-128">False</span><span class="sxs-lookup"><span data-stu-id="faa5a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="faa5a-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="faa5a-129">See also</span></span>



[<span data-ttu-id="faa5a-130">Getlembretes</span><span class="sxs-lookup"><span data-stu-id="faa5a-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="faa5a-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="faa5a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

